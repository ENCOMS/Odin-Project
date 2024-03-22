# Typical use cases

## [mdn/typical use cases of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Typical_Use_Cases_of_Flexbox)

flexbox is a layout, like the different type of layouts that exist in CSS.

flexbox have differences with the other layouts, as this seek to lay out the items one direction or another or control or spacing between items.

We use flexbox as fallback of CSS Grid layout and in order to get alignment capabilities.

## Flexbox for navigation

to display items as a horizontal bar.

## Space distributed outside the items

to distribute space between, around or evenly using the alignment properties in flexbox, and the justify-content.

## Space distributed inside the items

this can be done with the use of flex properties, that allow grow, shrink and size in basis of a hypotetical proportion.
Controlling ratios of flex items along the main axis.

## Split navigation

this use auto margins in the main axis.
and the use of gap properties

## Center an Item

this use flex containers, but later would be part of the block layout. for this we use inside the flex container the justify-content, align-items, align-self

## Card layout pushing footer down

can be done using changing the flex-direction to column

## Media objects

Media object is a common pattern in web design, this pattern has an image or other element to one side and text to the right. Ideally a media object should be able to be flipped, moving the image from left to right.

We see this in comments, and everywhere where we need to display images and descriptions.

for this we use flex: 1 and max-width

## Flipping the media object

for this we use flex-direction to row reverse.

## Form controls

We can give better style and behaviors using, controlling how much it can grow and shrink width flex properties.
