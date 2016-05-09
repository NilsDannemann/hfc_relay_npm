#Mediaqueries
Four sets of sass-mixins let you control the responsive flow of your document:

- **Above** a certain breakpoint (``` @include respond-above(breakpoint-name) { ... } ```)
- **Below** a certain breakpoint (``` @include respond-below(breakpoint-name) { ... } ```)
- **At** a certain breakpoint (``` @include respond-at(breakpoint-name) { ... } ```)
- **From** a certain breakpoint (``` @include respond-from(breakpoint-name, breakpoint-name) { ... } ```)

You can also pass a px value instead of a breakpoint-name.


<br><hr>
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


<br><hr>
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



<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `respond`, choose your type (above, below, at or between) and hit `TAB` to place your include.

<br><hr>
###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/wMRmrK?editors=1100)