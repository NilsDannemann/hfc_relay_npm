# Checkbox
Creaes an animated Checkbox via ::before or ::after.<br>

<br><hr>
###Example
```html
<label class="my-label">
	<input class="my-checkbox" type="checkbox"/>
	Checkbox
</label>
```
```sass
.my-checkbox {
  @include checkbox();
}
```


<br><hr>
###Basic Usage

```sass
// Simple Implementation
@include checkbox();

// How to change the Color?
@include checkbox($color: #fff);
```

###All the Options

```sass
@include checkbox(
  $color: $color-brand,
  $border: 2px solid $color-grey,
  $border-radius: 0px
); 
```


<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `overlay` and hit `TAB` to place your include.