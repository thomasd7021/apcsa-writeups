# Process Writeup

## Name: Thomas Dono
## Course: APCSA
## Period: 2
## Concept: Recursion

### Context
We just finished out final unit In our APCSA class in preperation for the AP test.

#### What We Learned
We learned about recurtion in java and how it works and can be used. Recurtion kind of sounds like repeat and that is what it does, recusion repeats the code over and over with out the need for a loop. Recurtion is when you call the function or method inside of its self. So if I want somthing to print out how many of each tens, thousands, millions in a number I can use a for loop to to that or I can use recurtion. That would look like this:

```java
public void digits(int a){
    if (a > 9){
        System.out.println(a);
    } else{
        digits(a/10);
        System.out.print(a);
    }
}
```
If I imput 123456789 then the out put would be 1, 12, 123, 1234, 12345, 123456, 1234567, 12345678, 123456789. This is because it needs to execute the full line before moving. So when the computer gets to execude the `digits(a/10);` line it needs to finish it before it can print what every a is. If a is greater 9 than i needs to keep executing `digits(a/10);` untill it is leading to the above resutls.

### Challange
One challenge I faced was on the unit test. I got 9 questions wrong and one that was the hardest for me was question 3. This was the question:

```java
Consider the following method.

public static void recurMethod(String str)
{
  if (str.length() > 3)
  {
    recurMethod(str.substring(2, str.length() - 2));
  }
  System.out.println(str);
}
Which of the following is printed as a result of the call recurMethod("programmers")

```

The right way to look at this is that `"programmers"` has more than 3 letters soit will cause the method to call its self but only passes a substring of `"ogramme"` this also has more than 3 letters soyou put it back through with a substring of `"ram"`.
When the check is made 3 is not greater than 3 so is continuew executing the code and prints out `"ram"`. Then we can do the rest of the code for the second time we call the method and print out `"ogramme"` then we can print out the lift time the method was called printing `"programmer"`. That was answer choice 3 but I choose answer choice 5 which was `"g"` `"ogr"` `"rogra"` `"programmers"`. 

### Takeaways
When trying to figur out the code on a test or for my self it makes more sence and is easier for me if I write out the code over and over and see how it works on paper. This will make it easier for me to visualize whats happening and more likely to get the right answer.
