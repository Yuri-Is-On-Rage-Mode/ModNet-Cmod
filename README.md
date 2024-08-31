# C% Language 🚀

C% is an advanced superset of C# that takes your development experience to the next level! Powered by `modnet`, C% offers enhanced performance, additional features, and unmatched versatility, making it the ultimate choice for modern developers.

## Features ✨

- **Seamless Integration:** Fully compatible with existing C# codebases and libraries.
- **Enhanced Performance:** Optimized for speed and efficiency with `modnet`.
- **Extended Syntax:** New language features and syntactic sugar for cleaner, more expressive code.
- **Cross-Compilation:** Easily convert your C% code into C# libraries or executables.
- **Multi-Format Output:** Produce both `.exe` and Windows executables, or generate `.netmodule` for modular development.
- **Rich Libraries:** Leverage a vast collection of built-in libraries to supercharge your projects.
- **Cross-Platform:** Write once, run anywhere with the power of `modnet`.

## Installation 📦

To get started with C%, you'll need to install `modnet`:

> just copy `MOD-NET` dir to your path.
- **EXAMPLE: `C:\Program Files\MOD-NET`**
```ps
Microsoft Windows [Version 10.0.19045.4780]
(c) Microsoft Corporation. All rights reserved.

C:\Program Files\MOD-NET\bin>dir
 Volume in drive C is SYSTEM_256M2
 Volume Serial Number is 3EEB-71D5

 Directory of C:\Program Files\MOD-NET\bin

24/08/2024  11:59 pm    <DIR>          .
24/08/2024  11:59 pm    <DIR>          ..
30/08/2024  12:09 am    <DIR>          C%-Compiler
25/08/2024  12:22 am    <DIR>          modnet_cli
               0 File(s)              0 bytes
               4 Dir(s)  102,700,572,672 bytes free

C:\Program Files\MOD-NET\bin>
```

## Getting Started 🛠️

- Create a file named `helloworld.cs`

**Start coding:**

```csharp
class Base {
public:
	virtual void VirtualMethod() {
		System.Console.WriteLine("Base::VirtualMethod");
	}
}

class Derived(Base) {
public:
	virtual void VirtualMethod() {
		System.Console.WriteLine("Derived::VirtualMethod");
	}
}

class A {
	shared void Main() {
		Base b = new Derived();
		b.VirtualMethod();
	}
}
```
## Compiling Your Code 🔧

```ps
PS G:\fri3nds\junk\modnet-lang\Samples\classes> modnet run virtual-specifier.cs
[*] Running CmodCompiler with virtual-specifier.cs...
[*] Output from CmodCompiler:
C%: @compiler: Compiling your masterpiece...
C%: @compiler: Compilation succeeded!
C%: @compiler: Total time: 00:00:01.0297324 - Fast, right?

@bye: That's all, folks! Exiting...

[*] Output from virtual-specifier.exe:
Derived::VirtualMethod

PS G:\fri3nds\junk\modnet-lang\Samples\classes> 
```

## Importing C# Libraries 📚

C% allows you to seamlessly import and use existing C# libraries:

```csharp
using Parent;

class A {
public:
	shared void Main() {
		Parent.Nested n = new Parent.Nested();
		n.Method();
	}
}
```
**COMPILES TO**
```ps
PS G:\fri3nds\junk\modnet-lang\Samples\classes> modnet run nested-declarations.cs
[*] Running CmodCompiler with nested-declarations.cs...
[*] Output from CmodCompiler:
C%: @compiler: Compiling your masterpiece...
C%: @compiler: Compilation succeeded!
C%: @compiler: Total time: 00:00:00.3705615 - Fast, right?

@bye: That's all, folks! Exiting...

[*] Output from nested-declarations.exe:
jUST IMPORTED C#'S CONSOLE LIB(.dll)!   

PS G:\fri3nds\junk\modnet-lang\Samples\classes> 
```

# ```CmodCompiler``` cli:
```ruby
PS G:\fri3nds\junk\modnet-lang\Samples\classes> CmodCompiler /h
Hamza Sufyan (Yuri), 2008-2088
CmodCompiler [options] [source-files]
/?                           Lists all compiler options
/keyfile:<file>              Specifies a strong name key file        
/lib:<dir1>[;<dir2>]         Specifies the location of referenced assemblies 
/out:<name>                  Specifies output assembly name
/ref:<file1>[;<file2>]       Imports metadata from the specified assemblies  
/ref:<alias>=<file>          Imports metadata using specified extern alias   
/t:exe                       Creates an executable (EXE), console application
/t:library                   Creates a dynamic-link library (DLL)
/t:module                    Creates a module without an assembly manifest   
/t:winexe                    Creates an executable (EXE), Windows program    

PS G:\fri3nds\junk\modnet-lang\Samples\classes>
```

## Community & Support 🤝

> We don't have a community yet—you're welcome to start the fan club!

## Contributing 🛠️

> Sorry, folks! This isn't open source... but nice try! 😆
