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

- ```grid-template-areas``` specifies grid named grid areas.
```css
.container
{
	grid-template-areas:	"a a"
							"b b"
							"c c"
}

.a {
	grid-area: a;
}
```

- grid layouts are two-dimensional: they have a row, or inline, axis and a column, or block, axis.

- ```justify-items``` specifies how individual elements should spread across the row axis.
```css
justify-items: start / end / center / stretch
```

- ```justify-content``` specifies how groups of elements should spread across the row axis.
```css
justify-content: start / end / center / stretch / space-around / space-between / space-evenly
```

- ```justify-self``` specifies how a single element should position itself with respect to the row axis.
```css
justify-self: start / end / center / stretch
```

- ```align-items``` specifies how individual elements should spread across the column axis.
```css
align-items: start / end / center / stretch
```

- ```align-content``` specifies how groups of elements should spread across the column axis.
```css
align-content: start / end / center / stretch / space-around / space-between / space-evenly
```

- ```align-self``` specifies how a single element should position itself with respect to the column axis.
```css
align-self: start / end / center / stretch
```

- ```grid-auto-rows``` specifies the height of rows added implicitly to the grid.
```css
grid-auto-rows: 'number'{px, %, fr, repeat()}
```

- ```grid-auto-columns``` specifies the width of columns added implicitly to the grid.
```css
grid-auto-columns: 'number'{px, %, fr, repeat()}
```

- ```grid-auto-flow``` specifies in which direction implicit elements should be created.
```css
grid-auto-flow: row / column / dense
```
