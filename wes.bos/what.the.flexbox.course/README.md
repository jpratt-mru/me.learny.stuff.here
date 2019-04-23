# Things I Learned

## The Resource

[What the FlexBox](https://courses.wesbos.com/account/access/5cb8a1ce85f96c03c1e40545)

## 02: Introduction to Flexbox

- parent container needs a `display: flex` (and the container takes up the whole parent width) or `display: inline-flex` (and container takes up content width only)
- immediate (only?) children are automatically made `flex items`
- (new thing to me) `vh` stands for "viewport height" and is a new unit of measurement like px and %. **100vh** would be "fill viewport vertically", **50vh** would be "fill 1/2 viewport", etc

## 03: Working with Flexbox flex-direction

- `flex-direction: row` (default) has the `major axis` moving horizontally across the viewport, left to right and the `cross axis` moving vertically top to bottom
- conversely, `flex-direction: column` has the major axis moving vertically top to bottom, and the cross axis moving left to right horizontally
- there is also `flex-direction: row-reverse` and `column-reverse`

## 04: Wrapping elements

- flex items that are too big are automatically scrunched to fit their container, but...
- you can use `flex-wrap: wrap` and items will do their best to take the width you give them and wrap all the items evenly in their parent
- there is also a `wrap-reverse` and the cross axis goes the opposite direction
- (new thing to me) `calc(100%/3) or calc(33.3333% - 20px)` could be used for units in CSS now 

## 05: Flexbox ordering

- `order: n` on a flex item will allow you to change its position is relative to its sibling items
  - so if you have a default of **order: 1** and then give somebody a **order: 2**, it will appear after the other sibs
- default is 0
- yes, negatives are possible and behave as expected