# Process Writeup

## Name: Thomas Dono
## Course: APCSA
## Period: 2
## Concept: Array Lists

### Context
I am in my APCSA class and we are currently learning java in preperation for the Ap exam in may.
#### What We Learned
We just learned about ArrayLists and how to sort through them. ArrayLists are like Arrays but they hold objects insted of variable. For example you can have an ArrayList of Car objects but not int values. However ArrayLists can hold Integer values because Integers are the object class for the int variable.

When you want declare an ArrayList you do `ArrayList<Object> name = new ArrayList<Objecct>();`. Where `Object` is the object that you want the ArrayList to hold and `name` being what you want to call the ArryList. Just like normal arrays, ArrayLists can hold as any many values as is needed. When we add a value we use the `.add()` method. There are 2 way to imploment the `.add()` method one just add the object to the end of the array and looks like this: `.add(objectName)` and the other let's you add the object to a sepesific index like this: `.add(i,objectName)` where it will insert `objectName` at index `i`. There are 4 other methods that are useful to ArrayLists: `.get(i)`, `.set(i,objectName)`, `.remove(i)`, and `.size()`. `.get(i)` will return the object at index i, `.set(i,objectName)` will overide the value at index `i` and sets it to `objectName`, `.remove(i)` removes the object at index i, and `.size()` returns the length ofthe array.

We also learned about sorting algortihms to help sort objects. The 3 sorts are the linear search, selection sort, and the insertion sort. They all work differently and can be used for differtn purposes. The linear search with go through every vlue untill the desired value is found and looks like this:
```java
for (int i = 0; i < length; i++)
{
  if (…)
  {
    return …
  }
}
```
A selection sort will sort the information by comparing the first value untill if finds a vlaue lower and seves thatas the new minimum untill if find one thats lower. Then it brings that value up to the front and repeats. The Insertion sort will check the first value and comare it to the value the its lft if its smaller it will swap them and continue to do that all the way down the array untill its fully sorted.
### Challange
One challenge I faced was reading code I didn't write. Question 3 on the quiz had this code to refer to questions 3-5:
```java
public class Whatchamacallit
{
  private double price;
  private String title;

  public Whatchamacallit()
  {
    this (0, "none");
  }

  public Whatchamacallit(double p, String t)
  {
    price = 0;
    if (p > 0)
    {
      price = p;
    }
    title = t;
  }

  public String toString()
  {
    return title + " costs $" + price;
  }
}
```
and
```java
ArrayList<Whatchamacallit> list = new ArrayList<Whatchamacallit>();

list.add(new Whatchamacallit());
list.add(new Whatchamacallit(3.5, "book"));
list.add(new Whatchamacallit(-17, "CD"));
list.add(new Whatchamacallit(18.95, "sweater"));
list.add(new Whatchamacallit(5, "notebook"));

/* Missing Code */
```
I got all the questions rong because I didnt read the code correctly. I miss read the second part and got them all wrong.

### Takeaways
I need to read more code from other people to help my brain see how it looks and better prosess code not just from others but from me as well.
