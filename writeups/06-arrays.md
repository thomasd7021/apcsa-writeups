# Process Writeup

## Name: Thomas Dono
## Course: APCSA
## Period: 2
## Concept: Arrays

### Context
I am learning Java in my APCSA class and we are about half way through the course. We just finished learning classes and how object based programming work. We are now learing Arrays.

#### What We Learned
 Arrays are like lists that hold many valuesand they can be changed and munipulatedtodo many things. We learned how to define an Array with `variable[] name = {values}`. Arrays also have ways that act on them so you can munipulate the array like  `name[i]` and `name.length()`.

When using an array you declare it the same as a variable but add bracket to the end of the variable type. It would look like this `int[]` but you still need to inisilize it. You can inisilize it in two ways the fists is like and object with the data type and a `new` prefix then you need to have the data type with the amount of values you want in the array. As an example, `int[] arr = new int[6]` this will make an array that can only take int values with 6 value spots for ints. The other way is withthe values like this `int[] arr = {10,12,18,5,6}`

There are many ways we learnd to modify arrays. One of them is the `name[i]`. This can be used as a variable with the value at the index `i` in the array. you can chnage it or use it to do math. touse this effectivly we can iterate through and array with a for loop. We want to make sure that we use it properly though or it might try to edit somthing thats not there. We make somthing like this.

``` java
for (int i = 0; i <= arr.length() - 1; i++)
{
  arr[i] = arr[i + 1];
}
```

This will go through the array items and change them to the vlaue after it but the last 2 values will be the same letting you change the last one toa different value.
### Challange

One challenge I have is reading code that I didn't. On the quiz at the of the unit thats most of the questions I got wrong. For example question 8 has this code

```java
public static boolean mystery(int[] nums)
{
  for (int i = 1; i < nums.length; i++)
  {
    if (nums[i] < nums[i - 1])
    {
      return false;
    }
  }
  return true;
}
```
It asked what the code does. I said it checks to see if the number after it is equal to the number before. This is the same idea but the wrong way. The class goes trhough the code and see if the index before it is that same as the one after.
### Takeaways

Key takeaways I have is that I need to read questions and code more carefully when I tkae tests and not stress asmuch on the time I have left. I can also make study sheets for the test that we have so I can study more have have help on the test.
