Halogen
=======

Delightful and performance-focused pure css loading animations. Inspired by [http://connoratherton.com/loaders]

## Demo & Examples

Live demo: [yuanyan.github.io/halogen](http://yuanyan.github.io/halogen/)

To build the examples locally, run:

```
npm install
gulp dev
```

Then open [`localhost:9999`](http://localhost:9999) in a browser.

## Installation

The easiest way to use `halogen` is to install it from NPM and include it in your own React build process (using [Browserify](http://browserify.org), etc).

You can also use the standalone build by including `dist/halogen.js` in your page. If you use this, make sure you have already included React, and it is available as a global variable.

```
npm install halogen --save
```

## Usage

```
var Halogen = require('halogen');
var Example = React.createClass({
    render: function() {
        var style = {
            width: 120,
            height: 120,
            display: 'inline-block'
        };
        return (
        <div>
            <div>
                <div style={style}><Halogen.BallPulseLoader color="#26A65B"/></div>
                <div style={style}><Halogen.BallGridPulseLoader color="#049372"/></div>
                <div style={style}><Halogen.BallClipRotateLoader color="#8DB255"/></div>
                <div style={style}><Halogen.SquareSpinLoader color="#8DB255"/></div>
                <div style={style}><Halogen.LineScaleLoader color="#006442"/></div>
            </div>
            <div>
                <div style={style}><Halogen.LineSpinFadeLoader color="#4DAF7C"/></div>
            </div>
        </div>
        );
    }
});
```
