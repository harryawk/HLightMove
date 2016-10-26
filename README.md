## HLightMove

is a running highlight for HTML element text, image, etc.

![capture](../img/optimised.gif "capture")

## Usage

### Creating instance

`new HLightMove(this_pointer, user_setting)`

`this_pointer` References to current/clicked anchor elements (required).

`user_settings` Setting for highlight instance and animation (oprional).

### Running instance

use `run()` method to move the highlight

### User Settings


| Option        | Value                                               |
| ------------- | --------------------------------------------------- |
| bgcolor       | css color, e.g. 'blue', rgba(0, 0, 0, 1), '#FFFFFF' |
| speed         | 'slow' &#124; 'normal' &#124; 'fast'                |


### Example

```
// example 1
// create instances
var hlightmove = new HLightMove(this);

// use run() method to move the highlight
hlightmove.run();

// example 2
// highlight on anchor element without user_setting
$('a').click(function(e){
	(new HLightMove(this)).run(); // this parameter is required
});

// example 3
// highlight on anchor element with user_setting
$('a').click(function(e){
	(new HLightMove(this, {
		'bgcolor': 'rgba(10, 200, 60, 0.8)',
		'speed': 'normal'
	})).run(); // this parameter is required
});
```

view me on [Github](https://github.com/riochr17)