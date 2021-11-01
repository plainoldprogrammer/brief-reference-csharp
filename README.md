# Brief Reference C#
Brief reference of the C# programming language.

---

#### Single line comment
```
// this is a single line comment
```

#### Use a namespace
```
using System;
```

#### Define a namespace
```
namespace CustomNamespace
{
}
```

#### Use a namespace
```
using CustomNamespace;
```

#### Define a class
```
public class SomeClass
{
}
```

#### Instantiate an object of a class
```
SomeClass someObject = new SomeClass();
```

#### Define a method
```
public void DoSomething()
{
}
```

#### Define a static method
```
public static void DoSomething()
{
}
```

#### Call to a method
```
DoSomething();
```

#### Define a static variable
```
public static float = 1.6;
```

#### Entry point of the application
```
public static void Main(String[] args)
{
}
```

#### Make nullable an integer
```
int? age = null;
```

#### Check if a nullable integer has a value
```
int? age = null;
age.HasValue.Dump();
```

#### Use the null coalescing operator
```
int? savingsAmount = null;
int? debit = 500;

int? available = savingsAmount ?? debit;
available.Dump();
```

#### Boxing
```
int age = 30;
Object someAge = age;
```

#### Preincrement
```
++someVariable;
```

#### Postincrement
```
someVariable++;
```

#### Enclose a class into namespace
```
namespace CustomNamespace
{
    public class SomeClass
    {
    }
}
```

#### Represent an integer big number in a friendly way
```
int number = 1_000_000;
```

#### Use the ternary operator
```
bool isValidId = true;
bool canDrive = isValidId ? true : false;
```

#### Inherit from a class
```
class ChildClass : ParentClass
{
}
```

#### Implement an interface
```
class SomeClass : IInterfaceToImplement
{
    void MethodToImplement()
    {
    }
}
```

#### Check if an object reference is null
```
if (someObject == null)
{
}
```

#### Create a list of strings
```
List<String> names = new List<String>();
```
####

#### Create an array of integers
```
int[] someYears = new int[] { 1986, 1989, 1999 };
```

#### Declare a const
```
public const double PI = 3.1416;
```

#### Print a message
```
Console.WriteLine("Hello!");
```

#### Read a line
```
string input = Console.ReadLine();
```

#### Cast a double to integer
```
double pi = 3.1416;
int value = (int) pi;
```

#### And operator
```
bool canDrive = hasGoodVision && isOlder;
```

#### Or operator
```
bool isEngineer = false;
bool isDeveloper = true;
bool canDevelopSoftware = isEngineer || isDeveloper;
```

#### Select all the elements from a collection
```
var result = someCollection.Select(x => x);
```

#### Verbatim string
```
int year = 2021;
@"Hi, currently is {year}!"
```

#### Get the type of an object
```
var i = 600;
Console.WriteLine("{0}", i.GetType());
```

#### Different ways of build a string
```
string name = "John Doe";
int age = 35;

Console.WriteLine(name + " is " + age + " years old");	// String concatenation
Console.WriteLine("{0} is {1} years old", name, age);	// Composite formatting
Console.WriteLine($"{name} is {age} years old");		// String interpolation
```

#### Collection initializer syntax
```
Ticket ticket1 = new Ticket { Description = "Udemy Course", Ammount = 11 };
Ticket ticket2 = new Ticket { Description = "Pluralsight Annual Suscription", Ammount = 299 };
Ticket ticket3 = new Ticket { Description = "Icecream", Ammount = 5 };

List<Ticket> tickets = new List<Ticket>()
{
    ticket1,
    ticket2,
    ticket3
};
```

#### Get the max id from a table
```
book.Id = bookshelfDbContext.Books.Max(x => x.Id);
```

#### Clear the screen
```
Console.Clear();
```

#### Get the type of the current instance
```
var i = 600;
Console.WriteLine("{0}", i.GetType());

NOTE: GetType is an instance method of the Object class.
```
