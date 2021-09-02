# Brief Reference C#
Brief reference of the C# programming language.

---

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
