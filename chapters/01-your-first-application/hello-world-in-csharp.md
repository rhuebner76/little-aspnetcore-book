## Hello World in C# #
Before you dive into ASP.NET Core, try creating and running a simple C# application.

You can do this all from the command line. First, open up the Terminal (or PowerShell on Windows). Navigate to the location you want to store your projects, such as your Documents directory:

```
cd Documents
```

Use the `dotnet` command to create a new project:

```
dotnet new console -o CSharpHelloWorld
```

The `dotnet new` command creates a new .NET project in C# by default. The `console` parameter selects a template for a console application (a program that outputs text to the screen). The `-o CSharpHelloWorld` parameter tells `dotnet new` to create a new directory called `CSharpHelloWorld` for all the project files. Move into this new directory:

```
cd CSharpHelloWorld
```

`dotnet new console` creates a basic C# program that writes the text `Hello World!` to the screen. The program is comprised of two files: a project file (with a `.csproj` extension) and a C# code file (with a `.cs` extension). If you open the former in a text or code editor, you'll see this:

**CSharpHelloWorld.csproj**

```xml
<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>net8</TargetFramework>
  </PropertyGroup>

</Project>
```

The project file is XML-based and defines some metadata about the project. Later, when you reference other packages, those will be listed here (similar to a `package.json` file for npm). You won't have to edit this file by hand very often.

**Program.cs**

```csharp
using System;

namespace CSharpHelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

`static void Main` is the entry point method of a C# program, and by convention it's placed in a class (a type of code structure or module) called `Program`. The `using` statement at the top imports the built-in `System` classes from .NET and makes them available to the code in your class.

From inside the project directory, use `dotnet run` to run the program. You'll see the output written to the console after the code compiles:

```
dotnet run

Hello World!
```

That's all it takes to scaffold and run a .NET program! Next, you'll do the same thing for an ASP.NET Core application.
