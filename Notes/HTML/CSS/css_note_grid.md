# CSS note grid

### __Review / Note__

- ```grid``` and ```inline-grid``` is to set up a grid.
```css
display: grid
display: inline-grid
```

- ```grid-template-colums``` defines the number and sizes of the columns of the grid.
```css
grid-template-columns: 'number'{px, %, fr} ...
```

- ```grid-template-rows``` defines the number and sizes of the rows of the grid.
```css
grid-template-rows: 'number'{px, %, fr} ...
```

- ```grid-template``` is a shorthand for defining both ```grid-template-columns``` and ```grid-template-rows``` in one line.
```css
grid-template: 'number'{px, %, fr} ... / 'number'{px, %, fr} ...
```

- ```row-gap``` puts blank space between the row of the grid.
```css
row-gap: 'number'{px, %, fr}
```

- ```column-gap``` puts blank space between the columns of the grid.
```css
column-gap: 'number'{px, %, fr}
```

- ```gap``` is a shorthand for defining both ```row-gap``` and ```column-gap``` in one line.
```css
gap: row-gap / column-gap
```

- ```grid-row-start``` and ```grid-row-end``` makes elements span certain rows of the grid.
```css
grid-row-start: 'number'
grid-row-end: 'number'
```
__Note__: ```grid-row``` is a shorthand.

- ```grid-column-start``` and ```grid-column-end``` makes elements span certain columns of the grid.
```css
grid-column-start: 'number'
grid-column-end: 'number'
```
__Note__: ```grid-column``` is a shorthand.

- ```grid-area``` is a shorthand for ```grid-row-start```, ```grid-column-start```, ```grid-row-end```, and ```grid-column-end```m all in one line.
```css
grid-area: grid-row-start / grid-column-start / grid-row-end / grid-column-end
```

- ```repeat(number, 'numer'{px, %, fr} ...)``` and ```minmax('number'px, 'number'px)``` is some utils function for grid.