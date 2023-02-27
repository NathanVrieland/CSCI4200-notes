# Other influences on language Design

## computer architecture 
- laguages are developed around the Von Neumann / stored program architecture 

## design methodologies 
- new methodologies led to new paradigmes which led to new languages
    - object oriented paradigm led to C++ which lead to Java

## Computer architcture influence 
- imperitive languages 
    - most dominant, are designed around the von neumann computers
    - data and programs stored in memory 
    - variable model memory cells 
    - assignment statmentes model piping
    - iteration is efficient because isntructions are pysically next to each other

## Programming Methodologies influence 
- 1950's 
    - people worried about machine efficiency 
- late 60's 
    - people efficiency beacme inportant 
        - better control structures 
        - top-down design 
- late 70's 
    - Procedure-oriented to data oriented 
    - data abstraction 
- Middle 80's 
    - object oriented programming 
    - data abstraction + inheritance + polymorphism 

# language catagories

## imperitive language
- describe how a program operates 
- use of statements 
- variables, assignments, iteration
- include 
    - object oriented langs
    - scripting langs
    - visual langs
    - C, Java, Perl, JS, visual BASIC .NET, C++

## Declaritive language 
- focus on what the program should accomplish 
- do not specify the order of execution of statements 
- include 
    - logical programming languages 
        - rules are specified in no particular order
    - Functional programming languages 
        - apply functions to given parameters 
    - database languges 
        - SQL
    - markup   
        - HTML, XML

# Language design trade off
- Reliability vs cost of execution
    - java makes a lot of reliable checks, but is slow 
- Readability vs writability 
    - APL provides many powerful operators, so it is very writable, but not very readable 
- Writabliity vs reliability 
    - C++ pointers are powerful but unreliable 

# implimentation methods 

1. compilation
2. Pure interpretation 
3. hybrid implementation 
4. Just-in-time compiler

## compilation 
- translate high level program into machine code 
- used in large commercial applications 
- slow compilation -> fast execution 

### has several components
- lexical analyzer 
    - converts characters into lexical units 
- syntax analyzer 
    - turns lexical uints into parse trees which represent the grammer of the program 
- intermediate code generator 
    - generates a code (assembly) between sorce code and machine code 
- semantics analyzer 
    - focuses on the meaning of the a strcuture 
- Optimizer
    - improves the program by making it smaller and faster 
- code generator 
    - generates the machine language 
- symbol table 
    - database of user defined names and types 

### additional terms
- linking and loading 
    - collecting system program units and linking them to a user program 
- load module 
    - the user and system code together 

## pure interpretation
- no translation
- executed by another program (the interpriter)
- used for small programs or when efficiency is not an issue 
- easier implimentation of programs 
- slower execution 
- statment decoding is the bottleneck of interpritation 
- provides a virtual machine for the language 
- requires more space 
    - source table is present during execution 
- rare now, mostly used for web programming 

## hybrid implementation 
- compromise between compilers and interpreters 
- high level language is translated into intermeiate language that is interpreted 
- faster than pure interpretation 
- Java, Perl

## Just-in-time compilers 
- initially translate programs to an intermediate laguage 
- then compiler subprograms as they are called 
- machine code kept for subsequent calls 
- widley used in java programs
- in essence, delayed compilers 

## prepocessors 
- used to specify code from other files 
- `#include`, `using`, etc.

# Programming environments 
- collection of tools used to facilitate software development
- UNIX 
- Microsoft Visual studio .NET
    - enviorment used to build languages in .NET
- Netbeans 
    - Java IDE