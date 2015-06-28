# grill
A [toast](https://github.com/daneden/Toast) [grill](http://dopm.github.io/grill). Simple grid and chaotic.

## Installation

Install with [component](http://component.github.io/) :

    $ component install dopm/grill

However, you can just grab the [css file](http://dopm.github.io/grill/grill.css) from GitHub. There is no dependency.

## How to bake
First, link to grill.css in your HTML document's head:

`<link rel="stylesheet" href="grill.css">`

then, wrap the container with a `.g` class, :

```css
<div class="g">
	<div class="c c-1-4">

	</div>
	<div class="c c-3-4">

	</div>
	<div class="c c-6-12">

	</div>
</div>
```

### Namespace
Grid namespace `g` 
Columns namespace `c`

```css
<div class="g">
	<div class="c c-{X}-{X}">
	...
```

### Push and pull columns

```css
<div class="g">
	<div class="c c-{X}-{X} c-ph-1-5">
	...
```

`c-ph-{X}-{X}` to push and
`c-pl-{X}-{X}` to pull

### Centered

Centers the column in the grid and clears the row of all other columns

```css
<div class="g">
	<div class="c c-{X}-{X} c-center">
	...
```

option:
`c-center` to centerd.
`c-first` displays the column as the first in its row.
`c-last` displays the column as the last in its row.
`c-ab` align column to the bottom.
`c-am` align column to the middle.

### Removes gutters from the columns

```css
<div class="g g-no-gutter">
	<div class="c c-{X}-{X}">
	...
```

See also demo [removes gutters from the columns](http://dopm.github.io/grill/no-gutter.html)

### Browser
The grill can be used on IE7 and modern browsers
