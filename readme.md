# Java

## Data Types

### Primitive Data Types

Primitive data types in Java are basic data types that can never be `null`. Their type names, such as 'int', start with a lowercase letter.

#### byte

The `byte` data type in Java is used to store whole numbers in the range of -128 to 127. It is typically employed when memory conservation is crucial. Example:

```java
byte temperature = 25;
```

#### short

The `short` data type is used to store whole numbers with a larger range compared to `byte` (-32,768 to 32,767). Example:

```java
short population = 30000;
```

#### int

The `int` data type is commonly used for storing integer values within a larger range (-2^31 to 2^31 - 1). Example:

```java
int numberOfStudents = 150;
```

#### long

The `long` data type is used for larger integer values that exceed the range of `int`. It can store values from -2^63 to 2^63 - 1. Example:

```java
long nationalDebt = 21500000000L;
```

#### float

The `float` data type is used for representing floating-point numbers (decimal numbers). It is suitable for scenarios where precision is not a critical concern. (6 to 7 decimal digits) Example:

```java
float discountPercentage = 5.5f;
```

#### double

The `double` data type is also used for floating-point numbers, providing greater precision compared to `float`. It is commonly used when higher precision is required. (15 decimal digits) Example:

```java
double piValue = 3.14159265359;
```

#### boolean

The `boolean` data type is used for representing boolean values, which can be either `true` or `false`. Example:

```java
boolean isJavaFun = true;
```

#### char

The `char` data type is used to store a single character. It can represent any Unicode character. Example:

```java
char grade = 'A';
```

### Non-Primitive Data Types

Non-primitive data types in Java can be `null`, and their type names start with an uppercase letter.

#### String

The `String` class in Java is used to represent sequences of characters. Strings are widely used for handling textual data. Example:

```java
String greeting = "Hello, Java!";
```

#### Array

An array in Java is a data structure that allows you to store multiple values of the same type under a single variable name. Arrays can be of primitive or non-primitive types. Example:

```java
int[] numbers = {1, 2, 3, 4, 5};
System.out.println(numbers[2]); // 3
System.out.println(numbers.length); // 5

for (int i = 0; i < numbers.length; i++) {
  System.out.println(numbers[i]);
}

for (int value : numbers) {
  System.out.println(value);
}
```

#### Class

The `Class` data type represents user-defined data types in Java. Classes are the building blocks of object-oriented programming and encapsulate data and behavior. Example:

```java
public class Car {
    String model;
    int year;
}

Car myCar = new Car();
myCar.model = "Toyota";
myCar.year = 2022;

Car myCar2 = new Car();
myCar.model = "Toyota2";
myCar.year = 2023;

```

#### Interface

An `Interface` in Java defines a contract for classes to implement. It specifies a set of methods that implementing classes must provide. Interfaces enable multiple inheritance and abstraction in Java. Example:

```java
public interface Shape {
    double calculateArea();
}

public class Circle implements Shape {
    double radius;

    @Override
    public double calculateArea() {
        return Math.PI * radius * radius;
    }
}
```