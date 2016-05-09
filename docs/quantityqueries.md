![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
# Quantity Queries
Change styles based on the quantity of Elements.<br>
**Example Usecase:** Too many Elements in a horizontal Navigation


###Usage

```sass
@include quantity-at(4) {...} 			// styles when exactly 4 elements
@include quantity-above(4) {...} 		// styles when more than 4 elements
@include quantity-below(4) {...} 		// styles when less than 4 elements
@include quantity-between(2,4) {...} 	// styles between 2 and 4 elements
```

<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `quantity`, choose your type (above, below, at or between) and hit `TAB` to place your include.

<br><hr>
###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/zryjQY?editors=1100)