# Process Writeup

## Name: Thomas Dono
## Course: APCSA
## Period: 2
## Concept: Java Unit 1 - Primitives

### Context

I am learning Java in an AP cours so that I can get a jump start on what a college workload/class might feel like.

#### What We Learned
We learned all about how to output code with `System.out.print()`,  variable types like `String` `int` `double` and `boolean`, how to get user imput with `Scanner`, how to do calculations with variables, and how to cast variables.

To use `System.out.print()` you need to put things into the () and it will output it as a String. If you want to just output a number like 12345 then it will look like this: `System.out.print(12345)`. With strings you you need to wrap them in quotes for them to out put properly like `System.out.print("My name is Thomas")`. If you want to output "This is a number: 25" however, you need to use concadination because you are using both strings and numbers. so it would look like this: `System.out.print("This is a number: " + 25)`.

When you want to declare a variable in JavaScript you do `var name` but in java you need to declare the data type of that variable. For words or a scentince it would be a `String` varibale. Numbers without decimals are `int` decimals are `double` and a true or false value is a `boolean`. They all can hold a limited amount of data which is why you need to declair the type before hand unlike JavaScript.

`Scanner` is a tool that takes what the user imputs and use them in the code. YOu have to declare it befoer you can useit though. to declare it you need to do `Scanner scan = new Scanner(System.in);` this will let you use user imputs. If you want a string from the user then you would declare the variable like this: `String name = scan.nextString;`. For the variable types just replase the `String` with what every the data type is.

You do variable calculations like normal calculations. So to add variable a and b you just do `a + b` and set it to a variable or put it in a print function. However, calculations with int variables will only get int variables so if `int a=13` and `int b=2` and you do `System.out.print(a/b);` your output will be 6 as 13/2 is 6.5 and its an int/int so it can only return a int variable. To help get around this we can use variable casting.
### Challange
The challenge I had this unit was understanding variable casting. I didnt undertand the use of casting double variables into int variable and not just haveing the vaiables be double variables at the start. For example:
``` java
Scanner scan = new Scanner(System.in);
   System.out.println("Please input two decimal numbers:");
   double o =  scan.nextDouble();
   double t =  scan.nextDouble();
   o = (int)o;
   t = (int)t;
   System.out.println("Answer: " + o + " + " + t + " = " + (o+t));
```
I didnt understand why they wanted me to have the double cast as int untill i looked at it more. When you cast and int you are able to round up if you add .5 to the number. Looking somthing like this,
``` java
Scanner scan = new Scanner(System.in);
   System.out.println("Please input two decimal numbers:");
   double o =  scan.nextDouble() + .5;
   double t =  scan.nextDouble() + .5;
   o = (int)o;
   t = (int)t;
   System.out.println("Answer: " + o + " + " + t + " = " + (o+t));
   ```

### Takeaways
My key takeaways are that if you get stuck you shoul reread the instructions and if that dosn't move anything forward rewatch/reread the lesson. This helped me a ton becase the first time I did Unit 1 Lesson 6 I just read the summary and understood it but not to the point I should have and strugled to do the coding activities. When I rewatched the video I was able to understand the code much better and I was able to do the activities fully and easily.