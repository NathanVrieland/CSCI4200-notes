# Language evaluaton Criteria (cont.)

## characteristics contributing to readability 
- overall simplicity 
    - Minimal operator  overloading 
        - (when a single operator has more than one meaning)
- Orthogonality 
    - small set of primitives combined in a small number of ways 
- data types 
    - Adequate for defining data structures 
- Syntax design 
    - special words (`while`, `class`, `for`, etc.)
    - compound statements (java's `else if`)
    - design statements so their appearence matches their purpose 
## characteristics contributing to Writability 
- simplicity and orthogonality
- expressivity
    - conveniesnt ways of expresing computations 
        - `count++` better than `count = count + 1`
## characteristics contributing to reliability
- type checking 
    - testing for type errors duing runtime or compile time 
    - compile time type cheking is less expensive and more desirable 
        - the earlier errors are detected, the better
- exception handling
    - correct run time errors with code 
    - present ing ada, c++, java, python, and C#
        - and in rust but I know you're using `unpack()`
    - not present in C and fortran
- Aliasing 
    - **negativley effects reliability**
    - presence of two or more distinct referencing methods for the same memory locations
        - present in C,C++,Java
- readability and writability 
    - if there is no 'natural' ways of expressing an algorithm, then unnnatural approaches will reduce reliabilty 
    - the easier a program is to write, the more likely it is to be correct 
## cost 
- training programmers is expensive 
    - simple programming laguages are cheaper to impliment
        - Go is easy to learn
- speed of writing a program 
    - time is money 
        - Go is concise and easy to write 
- compiling programs 
    - time is still money
        - Go has one of the fastest compilers
- executing programs
    - slow programs will take up too much time and money 
        - Go is so fast 
- Language implimentation 
    - avaliability of free compilers 
        - guess what Go is open source 
        - I like Go
- reliability 
    - critical faults are expensive to fix 
        - imagine a fault in a nuclear power plant or X-ray machine
    - non-critical faults can still cost buisness 
- Maintenance 
    - you need to hire programmers to fix faulty code 
        - rust gets this point 
    - maintenece costs = 4x development costs 
    - depends on readability 
### three most important contributers to cost 
- development
- maintenance 
- reliability 

# Other language evaluation criteria 
- portability 
    - ease of use across many different machines 
- Generality 
    - how many things you can do with it
- well-definedness 
    - completness of languages' official definition 

# final note 
- language design criteria are weighed differently based on persepctive 
    - language users concerned with readability and writablity 
    - designers concerened with widespread use 
    - implimentors concerened with difficulty of implimenting language 