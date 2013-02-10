## jQuery Dichotomy Plugin

### Usage

You can use Dichotomy plugins through JavaScript or the markup API.

#### JavaScript usage:

    $('.dichotomy').dichotomy()

#### Data-API usage:

    <div class="dichotomy" data-level="0"></div>

Images must place in next div if don't pass in options.

    <div class="dichotomy-images">
     <img src="2.jpg">
    </div>
 
 
### Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to `data-`, as in `data-animate="slideUp"`.

<table>
    <tr>
        <td><strong>name</strong></td>
        <td><strong>type</strong></td>
        <td><strong>default</strong></td>
        <td><strong>description</strong></td>
    </tr>
    <tr>
        <td>direction</td>
        <td>string</td>
        <td>'clockwise'</td>
        <td>Direction dividing block: clockwise or counterclockwise ('counter')</td>
    </tr>
    <tr>
        <td>duration</td>
        <td>number</td>
        <td>400</td>
        <td>Duration animation. Time in ms. You can use jquery option 'slow' and 'fast'</td>
    </tr>

    <tr>
        <td>animate</td>
        <td>string</td>
        <td>'fade'</td>
        <td>Type of animation: fadeIn-fadeOut, slideUp-slideDown ('slideUp') or from right to left ('slideSide')</td>
    </tr>

    <tr>
        <td>images</td>
        <td>array</td>
        <td>-</td>
        <td>Array of string path to background-image if image don't pass via markup</td>
    </tr>
</table>

### Methods

####.dichotomy(options)

Initializes the galery with an optional options object.

    $('.dichotomy').dichotomy({
        animate:'slideSide'
        });

####.dichotomy('divide')

Show next image

####.dichotomy('unite')
Remove last image


### Events

Dichotomy plugin have two ewents for hooking into functionality.

<table>
    <tr>
        <td><strong>event</strong></td>
        <td><strong>description</strong></td>
    </tr>
    <tr>
        <td>divide
        </td>
        <td>This event fires when next image is shown.
        </td>
    </tr>
    <tr>
        <td>unite</td>
        <td>This event fires when last image is removed.</td>
    </tr>
</table>

### jQuery Compatibility

Tested with jQuery 1.8.3 and next browser on Windows
* IE 7/8/9
* Chrome 24.0
* Opera 12.14
* Safari 5.1.7
* Firefox 10.0.1

Please tell about find bug with other browser or platform.

### License

Plugin licensed under the MIT license



