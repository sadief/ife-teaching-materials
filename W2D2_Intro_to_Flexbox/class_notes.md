Hey folks, great work tonight! Keep flexin'

Today we did:

#### Review

Quick review to look at:

- Indentation (great work spotting this right away)
- Naming our html elements with semantic tags
- Identifying the relationship between different elements (parents, children, siblings)
- _The Box Model_
  - Content
  - Padding
  - Border
  - Margin
  - You can use Dev Tools to view the box model on each element
  - Here's a good resource for remembering the [Box Model](https://medium.freecodecamp.org/css-box-model-explained-by-living-in-a-boring-suburban-neighborhood-9a9e692773c1)
- _The Display Property_
  - Block - takes up as much space as they can width-wise, but width and height can be applied
  - Inline - Only takes up as much space as they need, and width and height can be set
  - Inline-Block - Behaves like inline elements but you can set a custom width and height

#### Flexbox

- Flexbox solves a lot of historical issues that CSS has had with layouts. It's the first step to making our pages responsive and gives us better ways to change layouts without having to position each individual element.

- First thing we do is set the parent element as a flexbox by using:
  `display: flex`

### Flexbox Parent Properties

There are some flexbox properties that you can apply to the parent element to control the layout.

#### flex-direction

- row
- row-reverse
- column
- column-reverse

#### justify-content

- flex-end
- flex-start
- center
- space-between
- space-around
- space-evenly

#### align-items

- flex-end
- flex-start
- center
- baseline
- stretch

#### flex-wrap

- wrap
- no-wrap
- reverse

#### align-content

- flex-end
- flex-start
- center
- space-between
- stretch

### Flexbox Child Properties

Similarly there are properties that you can apply to the child elements

#### order

- order: -1
- order: 0
- order: 1
- (etc)

#### align-self

- flex-end
- flex-start
- center
- baseline
- stretch

#### flex-grow

- flex-grow: 2
- flex-grow: 5
- (etc)

#### flex-shrink

- flex-shrink: 2
- flex-shrink: 5
- (etc)

#### flex (grow, shrink, basis)

- flex: 1
- flex: 1 1 auto

If you haven't already done Flexbox Froggy, DO IT. I promise it will help!
