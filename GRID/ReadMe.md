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

### grid-column

it is the short hand to show g-c-s and g-c-e grid-column:1/3; means it started at grid line 1 and ended at grid line 3. and if you are not aware how many columns you have in the layout we can use -1 to define the g-c-e as the last grid line.
👉🏻 grid-row also work in the same way

## grid-template-areas:

this is the shorthand for all the layouts,
the values are the names which are to be passed to the children of that grid with the property grid-area,
it should look like this:-
grid-template-areas:
"h h h h h h h h h h m m"
"c c c c c c c c c c m m"
"f f f f f f f f f f m m";
childrens:-
.header {
grid-area: h;
}
.menu {
grid-area: m;
padding: 10px;
}
.content {
grid-area: c;
}
.footer {
grid-area: f;
}

to get the blank values, we can put dot . in those areas.

## Autofit and min max

we use these two properties to give the dynamic values to the grid,
giving value auto-fit helps the children to stretch-out to satisfy other grid rules without leaving any gaps in the view-port.

### implicit rows

to give rules to newly created rows created as a result to satisfy the grid-column rules, we want to use the css property as grid-auto-row or grid-auto-column and define its height or width. so that it always preserve this property.
and you can actually get rid of the previously written rule for the grid-template-rows as all the rows are going to get created implicitly
