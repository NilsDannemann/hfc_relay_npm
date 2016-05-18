# The Grid
The Grid is a **fraction-based** grid system and uses flexible sass-mixins instead of fixed classes.<br>

This approach has the following advantages over conventional grids:<br>

- **Flexibility** - just pass any ```$fraction``` and ```$gutter``` you like
- **Cleanliness** - keep your Markup clean and readable
- **Simplicity** - keep all styles & behavior in one place (separation of concerns)


<br><hr>
###Quick Example
```sass
.parent {
	@include flexbox();

	.children {
		@include column(1/4);
	}
}
```


<br><hr>
###Requirements
- Flexbox (use ```@include flexbox();``` on **parent element**)
- Row containers (working to get rid of those)


<br><hr>
###Usage

```sass
@include column(1/4);
@include column(2/9);
@include column(14/23);
```


<br><hr>
###Adding Gutters

By default a column has no gutters. You can add gutters like so:

```sass
@include column(1/6, $gutter: true); 		// adds global gutters (use: 'true' or 'false')
@include column(1/6, true); 				// shorthand 
```
**Note:** This uses the global ```$whitespace``` variable for gutters.

You can also specify your own gutters like so:
```sass
@include column(1/6, $gutter: 10px); 		// adds px gutters
@include column(1/6, $gutter: 2em); 		// adds em gutters
@include column(1/6, $gutter: 3%); 			// adds % gutters
@include column(1/6, $gutter: $var); 		// you can also use sass-variables
@include column(1/6, $gutter: $var/2); 		// you can even do math with them
```


<br><hr>
###Using !important

Simply pass a $important variable.

```sass
@include column(1/6, $important: true); 	// adds the !important
```


<br><hr>
###Beta: Adding Behavior

By default a column has no special behavior. You can add two different behaviors like so:

```sass
@include column(1/6, $gutter: true, $behavior: stacking);	// works
@include column(1/6, $gutter: true, $behavior: doubling);	// has some bugs
```
**Stacking:** Columns use the full width on the m breakpoint (common pattern) <br>
**Doubling:** Columns automatically respond to certain breakpoints (try it out to better understand)



<br><hr>
###Beta: Fixed & Auto Columns

Fixed Width-Columns can be used like so:

```sass
@include column(250px);
```

Auto Width-Columns can be used like so:

```sass
@include column();
```

**Warning:** Neither of those have access to gutters or behaviors! 



<br><hr>
###Snippets
The Snippets for Sublime Text are optional but make the workflow much faster. <br>
**Install:** [Download](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/snippets.zip) the Snippets and place them in your `(path_to_sublime)/Packages/User` folder.<br>
**Usage:** Just type `column` and hit `TAB` to place your include.

<br><hr>
###Playground
You can test the mixin over here:<br>
![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/code-playground.svg)
[Open Playground](http://codepen.io/NilsDannemann/pen/MKZQxe?editors=1100)