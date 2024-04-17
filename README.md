# triple

Read a file of triplets and outputs as a table

This input:

~~~
  r1,c1,1
  r1,c2,2
  r1,c3,3
  r2,c1,4
  r2,c2,5
  r2,c3,6
  r3,c1,7
  r3,c2,8
  r3,c3,9
~~~

Will output:
~~~
  ,c1,c2,c3
  r1,1,2,3
  r2,4,5,6
  r3,7,8,9
~~~

Note that it assumes only one value per row / column. By
default the row is the first column in the input data, the
column the second and the value the third. The comma is the
delimiter. The can be changed by passing the `-r`, `-c`, `-v` flags
to override the columns used for the row, column and value
columns.

By default output is suitable for a csv file, add `-md` to
output in markdown format
