# C# Code Snippets for Visual Studio
Drop the `*.snippet` files in this repo to your `\Documents\Visual Studio 20xx\Code Snippets\Visual C#\My Code Snippets` folder 

## internal abstract class
**Shortcut:** `classa`  
**Description:** This snippet creates a class definition for an internal abstract class placing the cursor on the class name like so    
```C#    
internal abstract class MyClass
{    
}
```
## internal sealed class  
**Shortcut:** `classis`  
**Description:** This snippet creates a class definition for an internal sealed class placing the cursor on the class name like so
```C#    
internal sealed class MyClass
{    
}
```
## readonly Property (Immutable Property)  
**Shortcut:** `propr`  
**Description:** This snippet creates an automatically implemented property with only a 'get' accessor
```C#
public int MyProperty { get; }
```
## public sealed exception With ExcludeFromCodeCoverage  
**Shortcut:** `exceptionex`  
**Description:** This snippet creates a public sealed exception with ExcludeFromCodeCoverage attribute
```C#
[ExcludeFromCodeCoverage]
public sealed class MyException : Exception
{
    public MyException() { }
    public MyException(string message) : base(message) { }
    public MyException(string message, Exception inner)
        :base(message, inner) { }
}
```
## Public method calls Abstract method with suffix of "Core"  
**Shortcut:** `callcore`  
**Description:** Code snippet for declaring a public method that in turn calls out to a virtual/abstract method with the same name with a suffix of "Core"

```C#
public void DoSomething(int value, string data)
{
    DoSomethingCore(value, data);
}

protected abstract void DoSomethingCore(int value, string data);
```
## Public (non void returning) Method in turn Calling an abstract "Core" method that retuns a value  
**Shortcut:** `callcorereturn`    
**Description:** Code snippet for declaring a public method that in turn calls out to a virtual/abstract method with the same name with a suffix of "Core". These methods return a value
```C#
public int GetSomething(int value, string data)
{
    return GetSomethingCore(value, data);
}

protected abstract int GetSomethingCore(int value, string data);
```
## Consle.Readline snippet  
**Shortcut:** `cr`  
**Description:** Code snippet for Console.ReadLine
```C#
Consloe.ReadLine();
```
## try - catch - finally  
**Shortcut:** `trycf`  
**Descrption:** Code snippet for try - catch - finally block
```C#
try
{
}
catch (Exception)
{
    throw;
}
finally
{
}
```