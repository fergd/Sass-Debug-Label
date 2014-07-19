Sass-Layout-Label
================

A simple labelling tool I use when laying out my web pages. Helps me keep track of what block level elements are doing. It's also useful when working with back-end devs. You can replace the attr() type with any attribute, such as data-roles, types, etc.

```sh
@mixin layout-labels($attr-type: attr(class), $debug-font-size: 1em, $debug-color: black, $debug-bg-color: yellow){
	&:after{
		content: $attr-type;
		font-size: $debug-font-size;
		font-family: serif;
		color: $debug-color;
		padding: 0.25em;
		background-color: $debug-bg-color;
	}
}
```