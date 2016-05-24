# Overlay
Add an animated hover-overlay to a container.<br>


<br><hr>
###Basic Usage

```sass
// simple implementation
@include overlay(); 

// How to change the Overlay Color?
@include overlay($color: #fff);								// hex, rgba or $variable

// How to change the Icon?
@include overlay($icon: '\f002'); 							// will be placed in :after content: ''
@include overlay($icon-color: #fff); 						// hex, rgba or $variable

// How to change the Icon font-size?
@include overlay($icon-font-size: 20px); 					// or use presets: xs, s, m, l, xl, xxl

// How to change width & height?
@include overlay($icon-width: 40px, $icon-height: 40px);	// or use presets: xs, s, m, l, xl, xxl
```

###All the Options

```sass
@include overlay(
  $overlay: true,						// set to 'false' for no overlay
  $overlay-color: $color-brand, 
  $overlay-opacity: 0.85, 
  $icon: '\f0da', 						// set to 'false' for no icon
  $icon-width: 40px,					// or use presets: xs, s, m, l, xl, xxl
  $icon-height: 40px,					// or use presets: xs, s, m, l, xl, xxl
  $icon-color: #fff,
  $icon-font-family: 'FontAwesome',
  $icon-font-size: 12px,				// or use presets: xs, s, m, l, xl, xxl
  $icon-border: 2px solid #fff,
  $icon-border-radius: 100%
); 
```


<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `arrow` and hit `TAB` to place your include.