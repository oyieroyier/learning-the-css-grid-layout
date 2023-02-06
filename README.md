# CSS GRID

##### Introduction:

These are my personal notes and code on learning the CSS grid.

The instructor for this lesson is **[Slaying The Dragon](https://www.youtube.com/watch?v=EiNiSFIPIQE).**

The code accompanying this is my own implementation of the class.

---

CSS Grids, unlike Flexboxes, are two-dimensional and we can place items on them not only vertically & horizontally but in any way we please.

Grids are made up of numbered _row lines_ and _column lines_ that make up cells.

### Deep-Dive

Given the following HTML code:

```html
<div class="container">
	<div class="boxes box1">
		<h2>Box 1</h2>
	</div>
	<div class="boxes box2">
		<h2>Box 2</h2>
	</div>
	<div class="boxes box3">
		<h2>Box 3</h2>
	</div>
	<div class="boxes box4">
		<h2>Box 4</h2>
	</div>
	<div class="boxes box5">
		<h2>Box 5</h2>
	</div>
	<div class="boxes box6">
		<h2>Box 6</h2>
	</div>
	<div class="boxes box7">
		<h2>Box 7</h2>
	</div>
	<div class="boxes box8">
		<h2>Box 8</h2>
	</div>
	<div class="boxes box9">
		<h2>Box 9</h2>
	</div>
	<div class="boxes box10">
		<h2>Box 10</h2>
	</div>
</div>
```

All the divs are inside a `container` class with each of the divs having both a general class of `boxes` and a unique `box` class numbered from 1 to 10.

They also each have a label "Box 1" all through to "Box 10".

Let's first give a background to the `boxes` class to make the individual boxes visible:

```css
.boxes {
	background: #ff42ff44;
}
```

This is how the page will now appear.

![](./images/CSS-GRID.png)

### Into the Grid

We now give the `container` the display of grid. At first nothing will happen.

That's because when we create a grid, we need to secify how many rows and columns it should create.

If we write this code, it will create a single column with a width of 100px.

```css
.container {
	display: grid;
	grid-template-columns: 100px;
}
```
![](./images/CSS-GRID%20(2).png)

If we write this, it will create three columns with a width of 100px each.

The number of 100px in the code represents as many columns.

```css
.container {
	display: grid;
	grid-template-columns: 100px 100px 100px;
}
```
![](./images/3_rows_100px.png)

If you call on the browser inspector, and hover over the `container` element, you will see the outline of the grids as shown above.

The same rule goes for the rows. The number of times you repeat a measurement unit as the values of the `grid-template-row` key determines the number of new rows to be created by the grid.


We want to create a grid with 6 rows of 150px height and 4 columns of 150px width.

```css
.container {
	display: grid;
	grid-template-columns: 150px 150px 150px 150px;
	grid-template-rows: 150px 150px 150px 150px 150px 150px;
}
```

When we call the browser inspector we see the outline of the four columns and 6 rows created by the grid.

![](./images/6-rows-4-cols.png)

There is a better way to write this but we shall get to it in a moment.