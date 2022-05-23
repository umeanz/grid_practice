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

