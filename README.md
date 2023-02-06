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
<div class="boxes box1">
	<h2>Box1</h2>
</div>
<div class="boxes box2">
	<h2>Box2</h2>
</div>
<div class="boxes box3">
	<h2>Box3</h2>
</div>
<div class="boxes box4">
	<h2>Box4</h2>
</div>
<div class="boxes box5">
	<h2>Box5</h2>
</div>
<div class="boxes box6">
	<h2>Box6</h2>
</div>
<div class="boxes box7">
	<h2>Box7</h2>
</div>
<div class="boxes box8">
	<h2>Box8</h2>
</div>
<div class="boxes box9">
	<h2>Box9</h2>
</div>
<div class="boxes box10">
	<h2>Box10</h2>
</div>
```

Let's first give a background to the `boxes` class to make the individual boxes visible:

```css
.boxes {
	background: #ff42ff44;
}
```

This is how the page will now appear(PS: I added the H1 prior.)

![](./images/CSS-GRID.png)

