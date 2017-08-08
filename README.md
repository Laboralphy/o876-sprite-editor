# html-responsive-stub
This is a STUB. With preconfigured index.html, css, for mobile-first applications.

## responsive classes
Documents are structured with rows and columns. A row may contain up to 12 columns.
The main idea of a responsive structure is that columns widths adapt to screen size.
A column width can be defined as 12 in small screens and 4 in large screens.

### defining rows and columns
A quick example :

```html
<div class="row">
	<div class="col lg-4 md-6 sm-12">
		<p>text 1</p>
	</div>
	<div class="col lg-4 md-6 sm-12">
		<p>text 2</p>
	</div>
	<div class="col lg-4 md-6 sm-12">
		<p>text 3</p>
	</div>
</div>
```

* class **row** defines a new row.
* class **col** defines a new column .
* class **lg-x** sets column size when screen is **large** and below. **x** varies from 0 to 12.
* class **md-x** sets column size when screen is **medium** and below. **x** varies from 0 to 12.
* class **sm-x** sets column size when screen is **small** and below. **x** varies from 0 to 12.
* class **xs-x** sets column size when screen is **extra small** and below. **x** varies from 0 to 12.

### defining offsets
Offsets are just empty invisible columns placed just before a visible columns. 

In the following example, the columns will be offset by 2 on large screens, and will not be offset on small and extra-small screens.
```html
<div class="row">
	<div class="col offset-lg-2 lg-8 offset-sm-0 sm-12">
		...
	</div>
</div>
```

## other classes

### links and buttons
Simply works like reglular links. Here is a couple of examples :

```html
<a class="btn" href="to/the/next/page">The next page</a>
<button>Action!</button>
```

You can "disable" buttons and link :
```html
<a class="btn disabled" href="to/the/next/page">Can't click</a>
```

### navigation bar
A navigation bar will display a line of links

```html
<nav>
	<ul>
		<li>
			<a class="btn" href="page1">Item 1</a>
		</li>
		<li>
			<a class="btn" href="page2">Item 2</a>
		</li>
		<li>
			<a class="btn disabled" href="page3">Item 3 is disabled</a>
		</li>
	</ul>
</nav>
```

### navigation list
Works like navigation bar but will display all links as list (vertically positioned). And all items will be 100% wide.

```html
<nav class="block">
	<ul>
		<li>
			<a class="btn" href="page1">Item 1</a>
		</li>
		<li>
			<a class="btn" href="page2">Item 2</a>
		</li>
		<li>
			<a class="btn disabled" href="page3">Item 3 is disabled</a>
		</li>
	</ul>
</nav>
```

### card
A card is a portion of document inside a round cornered box (and a shadow effect).
```html
<div class="row">
	<div class="col lg-12">
		<section class="card">
			<p>...</p>
		</section>
	</div>
</div>
```

### title
A title may be colored with one of these tints
* red
* blue
* green
* purple
* gray
* orange
* golden
* ...

```html
<h1 class="title red">Red Title</h1>
```

### aliases
| Class name   | Style                            | Use                                                                            |
|--------------|----------------------------------|--------------------------------------------------------------------------------|
| wrapper      | width: 100%;                     | When you want something being as wide as the column allows.                    |
| container    | max-width: 1240px; margin: auto; | When you want a container no larger than 1240px, and horizontally centered.    |
| font-bigger  | font-size: 1.25em                | When you want to write bigger                                                  |
| font-smaller | font-size: 0.75em                | When you want to smaller bigger                                                |
