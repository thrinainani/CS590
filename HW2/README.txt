unexpand command:

Expand copies files to output, with space characters to tabs characters. The number of tabs characters to be printed depend on given spaces can be given using the option "--tab".

For Example:

unexpand --tab=5 unexpandtest.txt

Here when ever there are 5 continues spaces that 5 spaces will be replaced by one tab.

Here are the modifications which I have done.

1.  If you gave any tab size we will execute
next_tab_column =  column + (tab_size - column % tab_size);
Instead of using this I am adding 100 to column.

2. If you column is less than tab then we will execute next_tab_column = tab;
insted of that I am giving that value is always 10.

