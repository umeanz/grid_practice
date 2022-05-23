# CSS Grid
- when make a grid have to consider margine, gutter, count of column.
- when using Grid better to use Wrraper tag to enclose whole componet. it make easier to handle inner component then just using div. 

 1. first we have to declare the 'display: grid;'( when declare grid, it is automatically change into block)
 2. have to manage the grid-gap, grid-template-columns, grid-template-row.
 3. have to put the value each colums and row 
 ```css
    //when 3x3 
    wrapper{
   grid-template-columns: 100px 100px 200px;
   grid-template-row: 100px 100px 200px
   }
   ```
    upper css will show 
    1st column 100x100px 100x100px 200x100px 
    2nd column 100x100px 100x100px 200x100px
    3rd column 100x200px 100x200px 200x200px
 
 4. question: if the group is not list format, is it not able to use nth-child? 

5. various format to make grid 
  ```css
    .container {
    grid: display; 
    gird-template-rows: 1fx 1fx 1fx; 
    grid-template-column: 20px 20px 20px;
    }
  ```
  ```css
    .container {
    grid: display; 
    gird-template-rows: repeat(3,1fx); 
    grid-template-column: repeat(3,1fx);
    }
  ```
  ```css
    .container {
      grid: display; 
      gird-auto-rows: repeat(3,1fx); 
      gird-auto-rows: repeat(3,1fx);
      //Automatically arrangement items
    }
  ```
  ```css
    item:nth-child(1) {
      grid-column-start: 1;
      grid-column-end: 3;
      grid-row-start: 1;
      grid-row-end: 3;
    }
  ```
  ```css
    item:nth-child(1) {
      grid-column: 1;
      grid-row: 3;
    }
  ```
  ```css
    item:nth-child(1) {
      grid-column: 1/span 2;
      grid-row: 1/ span3;
    }
  ```
  ```css
    .container {
      grid-template-areas:
        "header header header"
       " a     main    b "
       " .       .     . "
       "footer footer  footer";
     }
  ```
6. Grid component
  - Grid Container: Whole area of Grid 
  - grid Item: child of Grid container  
  - Grid Track: Grid's row and column 
  - Grid Cell: a vitual cell contain one item
  - Grid Line: dividing line
  - Grid Number: each line's number
  - Grid Gap: the gab between cell
  - Grid Area: the area sunrounded grid line ( 'one cell')


