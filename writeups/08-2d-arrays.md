# Process Writeup

## Name: Thomas Dono
## Course: APCSA
## Period: 2
## Concept: 2D Arrays

### Context
I am currently in an APCSA class learning java. We just finished with Array lists and are currently learning 2D Arrays.
#### What We Learned
2D Arrays are pretty similar to normal arrays. 2D arrays let you nest multiple arrays into one. They are more like the traditional array in math with rows and columns. To define 2D arrays they are similar to normal arrays but with 2 deffiners. You need to set the numbers of arrays and the number of indexes in the arrays, like this: `int[][] grid  = new int[4][3];`. This creates an array of int values with 4 rows and 3 columns or 4 arrays with 3 indexes in them. if you where to print the array it would look like this:
``` java
0 0 0
0 0 0
0 0 0
0 0 0
```
If we want to change the values you need to change the values individually and cant add or subtract to the length like in arrays. To change a value you need to do `grid[row][column] = x` where x is an int value you want to set the value to. I i want to change the 0 in row 3 column 3 to a 1 it would look like this  `grid[3][3] = 1`.

To iterate through the 2D array there are 2 main ways to do it, Row-Major and Column-Major. Row-Major is iterating through the rows then the columns and Column-Major is columns then rows. Iteration for Row-Major looks like this:
```java
for (int row = 0; row < grid.length; row++){
  for (int column = 0; column < grid[0].length; column++){
    // code to change/use the value in row,column
  }
}
```
and this is Column-Major:
```java
for (int column = 0; column < grid[0].length; column++){
  for (int row = 0; row < grid.length; row++){
    // code to change/use the value in row,column
  }
}
```
The main difference between the two is that Row-Major goes through the full row before moving to the next row and Column-Major goes through the full column before moving onto the next column.
### Challenge
Question 9 on the test gave me trouble but that was only because the `return result;` in III was inside the for loop and not outside. Question 20 gave me some trouble as well. The question was "Consider the following method, which is intended to return an array which contains the minimum elements in each of the rows of a 2-dimensional array... Which of the following could be used to replace /* missing code */ so that minRows will work as intended?" with the following code present:
```java
/** @param  mat a 2-dimensional array
 *  @return an array which contains the minimum elements of each row in mat.
 */
public double[] minRows(double[][] mat)
{
  double[] mins = new double[mat.length];

  for (int k = 0; k < mat.length; k++)
  {
    double localMin = mat[k][0];
    for (double num : mat[k])
    {
      /* missing code */
    }
    mins[k] = localMin;
  }
  return mins;
}
```
The answer I choose was:
``` java
if (num < localMin)
{
  localMin = mat[k][num];
}
```
The reason this is wrong is that `num` is a value in the array and can not be used as an index. This could cause an out of bounds error if the value is greater than the length of the array. The correct answer is:
```java
if (num < localMin)
{
  localMin = num;
}
```
### Takeaways
The main takeaway I have is to take more time on the test to read through the questions more thoroughly and to start making my one page cheat sheet during the lessons so it can be more detailed. I'm also going to put the test into my phone calendar so I don’t forget about the test and cram the period before trying to remember what I need for the test.

