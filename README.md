# Data Types

## Learning Goals

- Discuss why data types matter in Java.
- Learn about the different data types.

## Why does a variable have a type?

A variable has a type so that we can control what values can be assigned to it.
In our example, we expect the `name` to be a word. This is important because we
expect to be able to do specific things with specific variables based on their
type.

For example, say we want to store the height of a bicycle. Maybe we have two
variables called `myBike` and `yourBike`. We would expect to be able to
calculate whether our bikes are the same height. If they are, we could use each
other's bikes. This is easy to do if we know the height of the bike is a number:

- Take the number from the height of `yourBike`: `42`
- Subtract the height of `myBike`: `36`
- The result is `12`

Now imagine that instead of `42`, the height of `yourBike` is stored as `tall`.
What is `"tall minus 36` supposed to be? Type mismatches can cause a lot of
issues in programming, so Java guards against that by forcing us to specify a
type with each variable we define. This is why Java is considered a **strongly**
**typed programming language**.

Note that not all languages are "typed", meaning that not all languages force
variables to have types. Discussing the pros and cons of typed vs non-typed
languages is outside the scope of this course. Just know that Java is typed and
will therefore warn you when you try to perform operations on variables of
different types that are not compatible.

## Different Data Types

In the previous lesson, we saw that we defined the variable as such:

```java
String name = "Katie";
```

The first part of that statement is the type of variable, or the data type. In
this example, the data type is something called a `String`. We can set the value
of a `String` to words or a string of characters. But there are quite a few
other data types that a variable could be. For example, there are `int` data
types that hold whole numbers and `double` data types that hold decimal numbers.

Each data type can also be of a certain size. For example, an `int` and a `long`
can hold a whole number; but are a different size. So how do we measure the size
of a data type and how do we know which one to use?

Data types are measured based off of how much memory they can hold. We measure
this in **bytes**. A **byte** is equivalent to 8 **bits**. A bit is the smallest
unit of storage and can store one binary digit (0 or 1).

| Data Type | Size    | Description                                                                   |
|-----------|---------|-------------------------------------------------------------------------------|
| `boolean` | 1 bit   | Stores true or false values                                                   |
| `byte`    | 1 byte  | Stores whole numbers from -128 to 127                                         |
| `char`    | 2 bytes | Stores a single character or ASCII value                                      |
| `int`     | 4 bytes | Stores whole numbers from -2.147 x 10<sup>9</sup> to 2.147 x 10<sup>9</sup>   |
| `long`    | 8 bytes | Stores whole numbers from -9.223 x 10<sup>18</sup> to 9.223 x 10<sup>18</sup> |
| `float`   | 4 bytes | Stores fractional numbers up to a precision of 6 to 7 decimal digits          |
| `double`  | 8 bytes | Stores fractional numbers up to a precision of 15 decimal digits              |

When it comes to true/false values, we tend to use **boolean** as the data type.
When we want to store a letter or a single character, we use the data type
**char**. For whole numbers, we usually use **int** as the data type and
**double** for decimal values.

If we want to store a word or a sentence of words, we would use the data type
**String**.

A String is a little different from the above data types. All the above data
types in the table are **primitive types**. **Primitive data types** are
pre-defined in Java and stored within the memory stack. Non-primitive data
types or **reference data types** are stored slightly differently in memory in
that they point to objects in the heap space. We will talk more about memory in
a minute, but for now know that the two types are stored differently within
memory.

Now let us dive into what memory is and how it is used in Java!

## Resources

[Primitive Data Type table](https://www.w3schools.com/java/java_data_types.asp)
