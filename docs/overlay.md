# Overlay
Add an animated hover-overlay to a container.<br>
You don't have to import anything to use Icons from different sets.

<br><hr>
###Basic Usage

```sass
// Simple Implementation
@include overlay();                       // uses global variables from the config

// How to change the Overlay Color?
@include overlay($color: #fff);

// How to change the Icon?
@include overlay($icon: 'fa-search');     // use fontawesome
@include overlay($icon: 'ion-search');    // use ionicons
@include overlay($icon: 'li-magnifier');  // use linearicons
@include overlay($icon: false);	          // disable icon

// How to change the Icon font-size?
@include overlay($icon-font-size: 20px);  // or use presets: xs, s, m, l, xl, xxl

// How to change width?
@include overlay($icon-width: 40px);      // or use presets: xs, s, m, l, xl, xxl
```

###All the Options

```sass
@include overlay(
  $overlay: true,                   // set to 'false' for no overlay
  $overlay-color: $color-brand, 
  $overlay-opacity: 0.85, 
  $icon: 'fa-search',               // set css :after content, or set to 'false' for no icon
  $icon-color: #fff,
  $icon-font-family: 'FontAwesome',
  $icon-font-size: 12px,            // or use presets: xs, s, m, l, xl, xxl
  $icon-width: 40px,                // or use presets: xs, s, m, l, xl, xxl
  $icon-height: 40px,               // or use presets: xs, s, m, l, xl, xxl
  $icon-border: 2px solid #fff,
  $icon-border-radius: 100%
); 
```


<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `overlay` and hit `TAB` to place your include.