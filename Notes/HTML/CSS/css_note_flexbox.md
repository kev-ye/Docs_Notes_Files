# CSS note flexbox

### __Review / Note__

- __```Dislay: flex``` changes an element to a block-level container with flex items inside od it.__
``` css
dislay: flex;
```

- __```Display: inline-flex``` allow multiple flex containers to appear inline with each other.__
``` css
display: inline-flex;
```

- __```Justify-content``` is used to space items along the main axis__
``` css
justify-content: flex-start / flex-end / center / space-around / space-between
```

- __```Align-items``` is used to space items along the cross axis.__
``` css
align-items: flex-start / flex-end / center / baseline / stretch
```

- __```Flex-grow``` is used to specify how much space (and in what proportions) flex items absorb along the main axis.__
``` css
flex-grow: 'number' (default value is 0)
```

- __```Flex-shrink``` is used to specify how much flex items shrink and in what proportions along the main axis.__
``` css
flex-shrink: 'number' (default value is 1)
```

- __```Flex-basis``` is used to specify the initial size of an element styled with ```flex-grow``` and/or ```flex-shrink```.__
``` css
flex-basis: 'number'px
```

- __```Flex``` is used to specify ```flex-grow```, ```flex-shrink```, and ```flex-basis``` in one declaration.__
``` css
flex: value_of_flex-grow value_of_flex-shrink value_of_flex-basis / value_of_flex-grow value_of_flex-shrink / value_of_flex-grow value_of_flex-basis
```

- __```Flex-wrap``` specifies that elements should shift along the cross axis if the flex container is not large enough.__
``` css
flex-wrap: wrap / wrap-reverse / nowrap (default value & only necessary to override a wrap value set by a different CSS rule)
```
__Note__: The ```flex-wrap``` property is declared on flex containers.

- __```Align-content``` is used to space rows along the cross axis.__
``` css
align-content: flex-start / flex-end / center / space-between / space-around / stretch
```
__Note__: the ```align-content``` proprety is declared on flex containers.

- __```Flex-direction``` is used to specify the main and cross axes.__
``` css
flex-direction: row / row-reverse / column / column-reverse
```
__Note__: The ```flex-direction``` property is declared on flex containers.

- __```Flex-flow``` is used to specify ```flex-wrap``` and ```flex-direction``` in one declatation.__
``` css
flex-flow: value_of_flex-direction value_of_flex-wrap
```
__Note__: The ```flex-flow``` property is declared on flex containers.

- __Remark__

__Flex containers can be nested inside of each other by declaring ```display: flex``` or ```display: inline-flex``` for children of ferlx containers.__

