# Brief Reference C#
Brief reference of the C# programming language.

---

#### Single line comment
```
// this is a single line comment
```

#### Multi line comment
```
/*
This is a multi line
comment
*/
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

#### Evaluate if an object is null and assign another object
```
someObject ??= nonEmptyObject;
```

#### Use the object that is not null
```
someObject ?? otherObject
```

#### Check if an object is not null
```
Person p = new Person();

if (p is not null)
{
    doSomething();
}
```

#### Check if an object is null
```
Person p = new Person();

if (p is null)
{
    Console.WriteLine("p is null");
}
```

#### Check if an object type is of an specific class
```
Employee ceo = new Employee();

if (ceo is Employee)
{
    Console.WriteLine("the ceo is an employee");
}
```

#### Import a static class from a namespace
```
using static System.Console;
WriteLine("Hello World!");
```

#### Get the enumerator from an enumerable
```
var result = someCollection.GetEnumerator();
```

#### Skip the current interation of a loop using continue
```
for (int i = 0; i < 10; i++)
{
    if (i == 5)
    {
        continue;
    }
    
    Console.WriteLine(i);
}
```

#### Exit at the current iteration of a loop using break
```
for (int i = 0; i < 10; i++)
{
    if (i == 5)
    {
        break;
    }
    
    Console.WriteLine(i);
}
```

#### Print the application arguments
```
static void Main(string[] args)
{
    foreach (var arg in args)
    {
        Console.WriteLine(arg);
    }
}
```

#### Assign a variable its default value for its data type
```
string name = default;
int age = default;
object = someObject = default;
```

#### Use verbatim string and string interpolation
```
var operatingSystem = "Windows";
Console.WriteLine($@"Check c:\tmp\; directory on {operatingSystem}");

NOTE: The order of $ and @ doesn't matter.
```

#### Verify that a primitive data type has an alias
```
double pi = 3.1416;
Console.WriteLine(pi is System.Double);
```

#### Verify that primitive types inherits from ValueType
```
double pi = 3.1416;
Console.WriteLine(pi is System.ValueType);
```

#### Create a string from a list of char
```
var myString = new string(array1.ToArray());
```

#### Point an action to a method that returns void
```
public static void Main(string[] args)
{
    Action someFunc = SayHello;
    someFunc();
}

public static void SayHello()
{
    Console.WriteLine("Hello World!");		
}
```

#### Use positional parameters
```
public static void Main(string[] args)
{
    SayHello(lastName: "Doe", firstName: "John");
}

public static void SayHello(string firstName, string lastName)
{
    Console.WriteLine($"Hello, I'm {firstName} {lastName}");
}
```

#### Define an enum
```
enum Color
{
    Red = 1,
    Green = 2,
    Blue = 3
}

public static void Main(string[] args)
{
    Color importantMessage = Color.Red;
    if (importantMessage == Color.Red)
    {
        Console.WriteLine("There was an error");
    }
}
```

#### Define and use a tuple
```
var tuple = new Tuple<string, string, int>("John", "Doe", 95);
Console.WriteLine($"Hello, I'm {tuple.Item1} {tuple.Item2}, and I'm {tuple.Item3} years old");
```

#### Generate two different guids
```
var guid1 = Guid.NewGuid();
Console.WriteLine(guid1);

var guid2 = Guid.NewGuid();
Console.WriteLine(guid2);
```

#### Declare a list using collection initializer
```
List<string> cities = new()
{
    "Dallas",
    "San Antonio",
    "Houston",
    "Austin"
};
```

#### Execute code only in debug mode
```
if (Debugger.IsAttached)
{
    // code to execute
}
```

#### Pass variable number of parameters using the params keyword
```
public static void PrintNames(params String[] names)
{
    foreach (string name in names)
    {
        Console.WriteLine(name);
    }
}

public static void Main(String[] args)
{
    PrintNames("John, Jane, Joe");
}
```

#### Define an override an abstract class
```
public class Program
{
    public abstract class Human
    {
        public abstract void SayHello();
    }
    
    public class Person : Human
    {
        public override void SayHello()
        {
            Console.WriteLine("Hello World!");
        }
    }
    
    public static void Main(String[] args)
    {
        Person person = new Person();
        person.SayHello();
    }
}
```
