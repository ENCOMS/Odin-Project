# Topic: Axes on flexbox

[TOP/CSS-Foundation/Axes](https://www.theodinproject.com/lessons/foundations-axes)

## Objectives

The Two Axes of flex container
How to change those axes to arrange the content in columns instead of rows and vise-versa.

## Defaults of display: flex

### for flex container

```css
flex-direction: row;
flex-wrap: nowrap;
justify-content: flex-start;
align-items: stretch;
```

### for flex items

```css
flex-grow: 0;
flex-shrink: 1;
flex-basis: auto;
align-items: stretch;
```

## flex-direction: row

Is the default value of `display: flex`, this puts the main axis horizontal (left-to-right)

flex-basis will refer to width

## flex-direction: column

The column value change the axis direction from horizontal (row) to vertical (top-to-bottom)

flex-basis will refer to height

### Knowledge check

**How do you make flex items arrange themselves vertically instead of horizontally?**
changing to `flex-direction: column`
**In a column flex-container, what does flex-basis refer to?**
flex-basis refer to height if column or vertical axis.
**In a row flex-container, what does flex-basis refer to?**
flex-basis refer to width if row or horizontal axis.
**Why do the previous two questions have different answers?**
because of the change in axis, also change the flex-basis.
