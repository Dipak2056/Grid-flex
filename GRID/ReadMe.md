# Grid layout

1. Give display grid to the parent div

### 2. grid-template-columns ===>

    a. This property defines and set the width of the div.
    b. we can use the width in px, em, rem, or auto.
    c. For example if we have grid-template-columns: 100px auto 100px, the grid will have 3 columns with respective width.

### 3. grid-template-rows ===>

     a. This property defines and set the height of the div.
    b. we can use the height in px,  em, rem, or auto.
    c. For example if we have grid-template-rows: 100px auto 100px, the grid will have 3 columns with respective width.

### Fraction units(fr) / repeat

Instead of using other units to define the width or height of the div. Grid allows us to us 'fr' which splits the entire grid into the fraction and each column takes the defined value of fr.
For example- grid-template-columns : 1fr 1fr 1fr;
it means the enire grid is splitted into 3 equal fractions. However,
grid-template-columns : 1fr 2fr 1fr;
it means the entire grid is splitted into 4 fractions and second/middle fraction is twice as other two fractions.

### repeat

Instead of writing 1fr 1fr 1fr to specify three different columns we can use repeat(3,1fr);
first parameter is how many rows/columns and the second parameter is how wide or tall it should be.

### we can set both rows and columns at once so this can be taken as 2 dimensional layout.

### grid-template

1.  it is the shorthand to define both grid-template-rows and grid-template-column
2.  first part of this property is row and second part is column

## position and size of the Grid

Note:- 👉🏻refer to container grid-position class of div

### grid-column-start ==>

it refers to the grid line to start with, in 2 columns grid we have 3 grid line, 1 at start 1 at between and 1 at the end.

### grid-column-end ==>

it refers to the ending line where the grid child should end.
