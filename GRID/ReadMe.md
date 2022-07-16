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

### Fraction units

Instead of using other units to define the width or height of the div. Grid allows us to us 'fr' which splits the entire grid into the fraction and each column takes the defined value of fr.
For example- grid-template-columns : 1fr 1fr 1fr;
it means the enire grid is splitted into 3 equal fractions. However,
grid-template-columns : 1fr 2fr 1fr;
it means the entire grid is splitted into 4 fractions and second/middle fraction is twice as other two fractions.

### we can set both rows and columns at once so this can be taken as 2 dimensional layout.
