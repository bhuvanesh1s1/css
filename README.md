# Flexbox Layout - Quick guide

### Introduction

- Flexbox is a one-dimensional layout method for arranging items in rows or columns.
- Flex items (expand) to fill additional space or shrink to fit into smaller spaces.
- Flex layout gives container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes)
- **Note:** Flexbox layout is most appropriate to the components of an application, and small-scale layouts, while the Grid layout is intended for larger scale layouts

### How to check Browser Support:

- [caniuse.com](https://caniuse.com/)

### Handy guide to css flex-box:

- [css-tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN docs](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

### Emmet shortcuts:

- [Emmet docs](https://docs.emmet.io/cheat-sheet/)

### Flex model terms:

![Flex terms](./flex_terms.png 'Flex terms')

- The **main axis** is the axis running in the direction the flex items are laid out in (for example, as a row across the page, or a column down the page.) The start and end of this axis are called the main start and main end.
- The **cross axis** is the axis running perpendicular to the direction the flex items are laid out in. The start and end of this axis are called the cross start and cross end.
- The **parent element** that has **display: flex** set on it (the <section> with container class in our example) is called the **flex container.**
- The items laid out as flexible boxes inside the flex container are called **flex items** (the <div> elements with item-$ class in our example).

### Flex : container

Flex container parent element attribute definition

```
.container {
  display: flex; /* or inline-flex */
}
```

```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

#### Flex : gap

Space between flex items

- Row gap only is row-gap
- Column gap only is column-gap
- Together is defined in gap

```
.container {
  display: flex;
  ...
  gap: 10px;
  gap: 10px 20px; /* row-gap column gap */
  row-gap: 10px;
  column-gap: 20px;
}
```

<img src="./images/flex/gap-1.svg" width="563" height="333">

<!-- ![Flex gap](./images/flex/gap-1.svg 'Flex gap') -->

#### cross-axis [Y-axis] : align-items

```
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```

<img src="./images/flex/align-items.svg" width="563" height="333">

<!-- ![Align items](./images/flex/align-items.svg 'Align items') -->

#### cross-axis [Y-axis] : align-content

```
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
}
```

<img src="./images/flex/align-content.svg" width="563" height="333">

<!-- ![Align content](./images/flex/align-content.svg 'Align content') -->

#### main-axis [X-axis] : justify-content

```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
```

<img src="./images/flex/justify-content.svg " width="563" height="333">

<!-- ![Justify Content](./images/flex/justify-content.svg 'Justify Content') -->
