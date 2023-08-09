# Primitve vs Objects

## Explain the difference between an “int” and an “Integer” in Java


- **int** --> is a primitve data type in java and it represent a 32 bits being primitve data types does not hold methods with them
- **Integer** --> is a class in java language to be specific in java standard library.
 it's a wrapper class that provides object-oriented representation of 'int' since it's an object type it allows you to perform methods associated with the class.

## What is the default value for ints? Integers?

- Default value for int is **zero**. but if you try doing it on the compiler you will get a compilation error which is `variable num might not have been initialized`. From my searching that's due to java saftey and it helps prevent bugs that is caused from uninitialized variables

```
int num;
System.out.print(num);
-----------
output
-----------
variable num might not have been initialized
```

- Default value for Integer is **Null**. That's because every wrapper classes
the default value is **NULL**


## What is autoboxing? Unboxing?

- Autoboxing --> is the process of converting a primitive data type to it's corresbonding wrapper class 

```
int primitiveInt = 42;
Integer wrappedInt = primitiveInt; // Autoboxing
```

- unboxing --> is the proccess of converting the wrapper class to it's primitive data type

```
Integer wrappedInt = 42;
int primitiveInt = wrappedInt; // Unboxing
```

## List the three basic categories of exceptions

1. checked exception
2. Error
3. runtime exception

## What type of statement can you use to handle an exception?

`try-catch` is the statement where you can handle exceptions by enclosing the try block that may raise an exception which will be handled in catch code block.

## What is input from a Scanner broken down into?

By default, a scanner uses white space to separate tokens. (White space characters include blanks, tabs, and line terminators.)


## Things I want to know more about
 1. Reading more about wrapper class
 2. deep dive in exception handeling.