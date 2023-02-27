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
