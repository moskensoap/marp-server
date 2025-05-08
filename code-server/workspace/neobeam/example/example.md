---
marp: true
theme: neobeam
paginate: true
math: katex
footer: '**mikael-ros**
         **A modern take on the LaTeX beamer theme**
         **Version 0.7, 2024**'
---
<!-- _class: title -->
# A modern take on the LaTeX beamer theme

## mikael-ros

> ### Faculty of GitHub
> University of Marp

## Version 0.7, 2024

![logo GitHub Logo](../assets/github-mark.svg)

---
<!-- header: 'Table of contents' -->
1. Normal text
2. Code blocks
3. Mathematics
4. Tables
5. Images
6. HTML stuff
---
<!-- header: 'Normal text' -->
**This** is what a regular slide can look like in Neobeam.
- A cool fact
- Interesting tidbit

My favorite letters are:
1. A
2. B
3. C

A quote from my favorite author
> "Hello" - Author Cool 2024

---
<!-- header: 'Code blocks' -->
We can define ``variables`` inline, and code in blocks (with syntax highlighting!!!):
```java
    if (marp) {
        apply.neobeam();
    }
```
---
<!-- header: 'Mathematics corner' -->
## Formulas
> The length of a vector can be computed by the following formula
> $$
||\overline v|| = \sqrt{a^2 + b^2} \\
\text{where } \overline v = (a,b)
$$
## Definitions
Blockquotes with level 4 (####) headings inside get translated to definitions like:

> #### Vector
> A collection of numbers

---
<!-- header: 'Data' -->
Tables are also decorated in this theme!
| Left Row    | Center Row  | Right row     |
| :---        |    :----:   |          ---: |
| Some        |  Cool       | Data          |
| Some        |  Cool       | Data          |
| Some        |  Cool       | Data          |
| Some        |  Cool       | Data          |
---
<!-- header: 'Images' -->

![Photo by Joshua J. Cotten on Unsplash](https://images.unsplash.com/photo-1601247387326-f8bcb5a234d4?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D) 

Images can be left-aligned, centered, and right-aligned!

---
<!-- header: 'HTML wonderland' -->
<!-- This slide only works with HTML enabled -->

<h2>These are all the HTML elements I've styled!</h2>

Text can be <mark>marked</mark>, <abbr title="abbreviated">abbr</abbr> and you can quote things inline <q>like this</q>.

You can embed audio like:
<audio controls src="http://codeskulptor-demos.commondatastorage.googleapis.com/pang/pop.mp3" type="audio/mp3">
</audio> 

---

<!-- header: 'Images with style' -->

<style>
.float-image1 {
  position: absolute;
  width: 15%;
  bottom: 5%;
  right: 15%;
  opacity: 1;
  box-shadow: 0 0 10px rgba(0,0,0,0.3);
}
</style>
<img src="../assets/github-mark.svg" class="float-image1"/>

<style>
.float-image2 {
  position: absolute;
  width: 15%;
  top: 5%;
  left: 15%;
  opacity: 0.5;
}
</style>
<img src="../assets/neobeam.png" class="float-image2"/>

<style>
.float-image3 {
  position: absolute;
  width: 200%;
  transform: translate(-50%, -50%); /* Shift the image so that its center aligns with the top-left anchor point */
  top: 50%;
  left: 50%;
  opacity: 1;
}
</style>
<img src="../assets/neobeam.png" class="float-image3"/>

<!--
## CSS `position` values explained:

- `static` (default): Elements are positioned according to the normal document flow. `top`, `right`, `bottom`, and `left` have no effect.
- `relative`: The element is positioned relative to its normal position. You can use `top`, `left`, etc. to "nudge" it.
- `absolute`: The element is positioned relative to the nearest positioned ancestor (non-static). If none, it's relative to the slide.
- `fixed`: The element is positioned relative to the viewport (the visible area). It stays in place even when scrolling.
- `sticky`: The element toggles between `relative` and `fixed`, depending on scroll position. Less common in Marp usage.

In Marp slides, `absolute` is most useful for precisely placing elements like images or text anywhere on the slide.
-->

---


<style>
.center-container {
  display: flex;                /* Specifies the layout of a container using Flexbox.
                                 * Other values: 
                                 * - block: default block-level container 
                                 * - inline: behaves like an inline element 
                                 * - inline-block: acts like a block element, but only takes up as much width as it needs 
                                 * - grid: for CSS Grid layout */
  
  justify-content: center;      /* Aligns child elements horizontally within the container.
                                 * Other values:
                                 * - flex-start: Aligns to the start of the container
                                 * - flex-end: Aligns to the end of the container
                                 * - center: Aligns to the center of the container
                                 * - space-between: Distributes space evenly between items
                                 * - space-around: Distributes space around items */
  
  align-items: center;          /* Aligns child elements vertically within the container.
                                 * Other values:
                                 * - flex-start: Aligns to the start of the container
                                 * - flex-end: Aligns to the end of the container
                                 * - center: Aligns to the center of the container
                                 * - baseline: Aligns to the baseline of text (useful for mixed content)
                                 * - stretch: Stretches the child elements to fill the container's height (default) */
  
  height: 100%;                 /* Sets the height of the container to 100% of its parent's height.
                                 * Other values:
                                 * - px: Fixed pixel values (e.g., 500px)
                                 * - vh: Percentage of the viewport height (e.g., 50vh is 50% of the viewport height)
                                 * - %: Percentage of the parent container's height
                                 * - auto: Automatically adjusts based on the content size */
}
.center-container img {
  width: 10%;                   /* Sets the width of the images inside the container.
                                 * Other values:
                                 * - px: Fixed pixel values (e.g., 200px)
                                 * - %: Percentage of the parent container's width
                                 * - vw: Percentage of the viewport width (1vw = 1% of the viewport width)
                                 * - auto: Automatically adjusts to maintain the image's aspect ratio */
}
</style>

<div class="center-container">
  <img src="../assets/neobeam.png" />
  <img src="../assets/github-mark.svg"/>
</div>


<style>
.center-container2 {
  display: block;
  justify-content: bottom;
  align-items: left;
  height: 100%;
}
.center-container2 img {
  width: 20%;
}
</style>

<div class="center-container2">
  <img src="../assets/neobeam.png" />
  <img src="../assets/github-mark.svg"/>
</div>

<style>
.center-container3 {
  position: absolute;           /* Absolute positioning */
  top: 80%;                     /* Position 80% from the top */
  left: 80%;                    /* Position 80% from the left */
  display: flex;                /* Still using flex layout */
  align-items: center;          /* Center images vertically within the container */
  justify-content: center;      /* Center images horizontally within the container */
  height: 20%;                  /* Optional, to define container height */
}

.center-container3 img {
  width: 20%;                   /* Sets the width of images */
}
</style>

<div class="center-container3">
  <img src="../assets/neobeam.png" />
  <img src="../assets/github-mark.svg"/>
</div>

---

<!-- header: 'Two-Column' -->

<style>
.columns {
  display: flex;           /* Flexbox layout to create columns */
  gap: 2em;                /* Space between columns */
}
.column {
  flex: 1;                 /* Each column takes equal space */
}
</style>

# Example: Two-Column Layout

<div class="columns">
  <div class="column">

### Left Column Title

- This is the content for the left column
- Continuing with a Markdown list
- Supports equations: $E = mc^2$

  </div>

  <div class="column">

### Right Column Title

1. This is the content for the right column
2. Supports numbered lists
3. Supports equations:

$$
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
$$

  </div>
</div>

<img src="../assets/neobeam.png" class="float-image2"/>

---

<style>
.columnsother {
  display: flex;           /* Flexbox layout to create columns */
}
.columnleft {
  width: 30%;              /* take 30% of the width */
}
.columnright {
  width: 70%;              /* take 70% of the width */
}
</style>

# Example: Two-Column Layout (Fixed Width)

<div class="columnsother">
  <div class="columnleft">

### Left Column Title

- This is the content for the left column
- Continuing with a Markdown list
- Supports equations: $E = mc^2$

  </div>

  <div class="columnright">

### Right Column Title

1. This is the content for the right column
2. Supports numbered lists
3. Supports equations:

$$
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
$$

  </div>
</div>

---

<style>
.columns-vertical {
  display: flex;
  flex-direction: column;  /* Stack the items vertically */
  height: 100vh;            /* Ensure the layout takes the full viewport height */
}
.column-top {
  height: 40%;             /* Top section takes 40% of the height */
  padding: 20px;
  background-color: #f0f0f0;  /* Light background for visibility */
}
.column-bottom {
  height: 50%;             /* Bottom section takes 50% of the height */
  padding: 20px;
  background-color: #e0e0e0;  /* Light background for visibility */
}
</style>

# Example: Two-Column Vertical Layout (Top-Bottom)

<div class="columns-vertical">
  <div class="column-top">

This is the content for the top section

Supports equations: $E = mc^2$

Markdown content, images, etc.

  </div>

  <div class="column-bottom">

This is the content for the bottom section

Supports equations:

$$ \int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2} $$

  </div>
</div>
