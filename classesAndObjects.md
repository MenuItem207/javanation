# Classes and Objects
These are two main aspects of object-oriented programming

## A world without classes
Let's say we want to represent 'people' programmatically, we'd first list out 'attributes' of the 'people' we want to represent:

### Name
Probably a string used to store a person's name

### Age
Probably an int used to store a person's age

### Ethnicity
Probably a string used to store a person's race

Maybe we'd use Arrays to store our data (not written in actual code):
```
person1 = ['bob', 12, 'chinese']
person2 = ['sally', 1, 'chinese']
```

These arrays create separate instances of 'people' that can be accessed like so:
```
// the name of person 1 is:
person1[0] // bob

// the ethnicity of person2 is:
person2[2] // chinese
```

This is not so great because theres no 'template', no 'structure' to refer to. We'd have to remember which 'index' each value is and also make sure to only put each value at the right place. If only we could do something like... 
```
person1.name // bob

person2.ethnicity // chinese
```

Wait. We CAN :D

## Classes
Classes are object templates, blueprints for constructing objects. To create a class, use the keyword class and make sure to aways start your classname with an uppercase first letter

```
public class ClassName {
    int classAttributeOne = 5;
    
    public static void classFunction() {
        System.out.println("hiii");
    }
}
```

Once we've defined our object template, we can create an INSTANCE of the template

## Objects
Objects are created from a class
```
ClassName object1 = new ClassName(); // create new INSTANCE of a 'ClassName' object using the 'ClassName' template'
System.out.println(object1.classAttributeOne); // 0 (default value)

ClassName object2 = new ClassName();
object2.classAttributeOne = 10;
System.out.println(object2.classAttributeOne); // 10

System.out.println(object1.classAttributeOne); // what value is this?
```

## Test
Imagine you are tasked with creating a simple program to manage a library system. Write Java code that demonstrates the use of a class to represent a Book with attributes such as title, author, and publicationYear. Instantiate two objects of the Book class and print out their details. Explain how using classes enhances the organization and readability of your code in this scenario.