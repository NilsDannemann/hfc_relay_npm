#Button
**Basic Button**
```sass
@include button();
```

###All the Options

```sass
@include checkbox(
  $size: xl, // optional presets: xs, s, m, l, xl, xxl
  $style: outlined, // filled or outlined (default: filled)
  $color: #fff, 
  $background: $color-brand, 
  $font-size: $font-size-m, 
  $padding: 10px 20px,
  $margin: 0 0 10px 0,
  $border: $border, 
  $border-radius: $border-radius,
); 
```

<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `button` and hit `TAB` to place your include.