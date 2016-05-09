# CSS Arrows
Use css-arrows via sass-mixins.<br>


<br><hr>
###Usage

```sass
// centered up-arrow
@include arrow(); 
// right-aligned down-arrow
@include arrow($direction: down, $align: right);
// top-aligned left-arrow with specific color & size
@include arrow($direction: left, $align: top, $color: #eee, $size: 10px);
```


<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `arrow` and hit `TAB` to place your include.

<br><hr>
###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/RrEJPL/?editors=1100)