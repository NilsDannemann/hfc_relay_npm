# Icon
Adds an Icon to current element via ::before or ::after.<br>
Automatically detects the used Icon-Set.

<br><hr>
###Basic Usage

```sass
// Simple Implementation
@include icon();

// How to change the Icon Color?
@include icon($color: #fff);

// How to change the Icon?
@include icon($icon: 'fa-search');     // use fontawesome
@include icon($icon: 'ion-search');    // use ionicons
@include icon($icon: 'li-magnifier');  // use linearicons

// How to change the Icon font-size?
@include icon($font-size: 20px);  // or use presets: xs, s, m, l, xl, xxl
```

###All the Options

```sass
@include icon(
  $icon: 'fa-search',               // set css :after content, or set to 'false' for no icon
  $color: #fff,
  $font-size: 14px,                 // or use presets: xs, s, m, l, xl, xxl
  $position: 'after',               // before/after
  $margin: 0 10px 0 0,              // adds margin
  $padding: 5px,               		// adds padding
); 
```


<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `overlay` and hit `TAB` to place your include.