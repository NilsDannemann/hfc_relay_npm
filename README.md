# HFC Relay Framework






<br><br><br><br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
<hr>
# Installation

## Via npm
1. Install: ```npm install hfc-relay --save-dev;```
1. Import: ```@import 'node_modules/hfc-relay/src/hfc-relay.scss';```

This approach has the following advantages over conventional grids:<br>











- [The Grid](docs/grid.md)









<br><br><br><br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
#Responsive Mixins
Four sets of sass-mixins let you control the responsive flow of your document:

- **Above** a certain breakpoint (``` @include respond-above(breakpoint-name) { ... } ```)
- **Below** a certain breakpoint (``` @include respond-below(breakpoint-name) { ... } ```)
- **At** a certain breakpoint (``` @include respond-at(breakpoint-name) { ... } ```)
- **From** a certain breakpoint (``` @include respond-from(breakpoint-name, breakpoint-name) { ... } ```)

You can also pass a px value instead of a breakpoint-name.



###Usage

**Above** a certain breakpoint (mobile-first)
```sass
.foo {
	//styles
	@include respond-above(xs) { ... }				// accpets breakpoint-names: xs, s, m, l, xl, xxl
	@include respond-above(500px) { ... }			// or specific px value
}
```

**Below** a certain breakpoint (desktop-first)
```sass
.foo {
	//styles
	@include respond-below(xs) { ... }				// accpets breakpoint-names: xs, s, m, l, xl, xxl
	@include respond-below(500px) { ... }			// or specific px value
}
```

**At** a certain breakpoint<br>
```sass
.foo {
	//styles
	@include respond-at(xs) { ... }					// accepts breakpoint-names: xs, s, m, l, xl, xxl
	@include respond-at(500px) { ... }				// or specific px value
}
```

**Between** two breakpoints<br>
```sass
.foo {
	//styles
	@include respond-between(xs, m) { ... }			// accepts breakpoint-names: xs, s, m, l, xl, xxl
	@include respond-between(500px, 900px) { ... }	// or two specific px values
}
```



###Placement
You can use the breakpoint-mixins in two ways:

Either inside your class-declarations...
```sass
.foo {
	color: red
	@include respond-above(l) { color: blue }
}
```

... or on their own.
```sass
.foo {color: red}
@include respond-above(l) { 
	.foo { color: red }
}
```
Both is fine.




###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `respond`, choose your type (above, below, at or between) and hit `TAB` to place your include.

###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/wMRmrK?editors=1100)


















<br><br><br><br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
# Position Shorthand
Use position relative, absolute or fixed in shorthand.<br>



###Usage

```sass
// shorthand
@include position(relative, 10px, 0, 0, 0);

// returns
position: relative;
top: 10px;
right: 0;
bottom: 0;
left: 0;
```


###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `position` and hit `TAB` to place your include.

###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/XXajGM?editors=110)








<br><br><br><br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
# CSS Arrows
Use css-arrows via sass-mixins.<br>



###Usage

```sass
// centered up-arrow
@include arrow(); 
// right-aligned down-arrow
@include arrow($direction: down, $align: right);
// top-aligned left-arrow with specific color & size
@include arrow($direction: left, $align: top, $color: #eee, $size: 10px);
```



###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `arrow` and hit `TAB` to place your include.

###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/RrEJPL/?editors=1100)








<br><br><br><br>
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


###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `quantity`, choose your type (above, below, at or between) and hit `TAB` to place your include.


###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/zryjQY?editors=1100)











<br><br><br><br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/devices.jpg)
#Other


###Container
**Basic Container**
```sass
@include container();
```



###Flexbox 
**Use Flexbox**
```sass
@include flexbox();
```