# Data Types 
# Variables
- abstraction of memory cell or collection of cells
- often thought of as names for memory locations, but there is more to it than that
- sextuple of atributes 
    1. Name: identifier associated with the variable 
    2. Address: memory address which the variable is associated, this can vary throughout execution
    3. Type: determines the range of values the variable can store 
    4. Value: the contents of the memory cell
    5. lifetime: the time the vairable is bound to the memory location
    6. Scope: range of statements that the variable is visible 

# binding 
- an association between an entity and an attribute 
    - variable and its type
    - symbol and its operation 
- binding time is the time at which it takes place 

## possible binding times 
- language design time 
    - bind operator symbols to operations 
- lang imnplimentaion time
    - bind types to representations 
- compile time 
    - bind variables to types 
- load times 
    - bind static variables to memory cells
- runtime 
    - binmd nonstatic local variables to memory cells 

## static vs dynamic bindings
- static 
    - occurs before run time and remains unchanged
- dynamic 
    - occurs during execution or can change during execution 
```
int count;
count = count + 5;
```
- the set of possible values for `int` is bound at compiler design time 
- the type of `count` is bound at compile time
- the meaning of `+` is bound at compile time 
- the meaning of the literal `5` is bound at compiler design time
- the value of `count` is bound at execution time

## data types 
- defines a collection of data and predefined operations 
    - int is collection of whole numbers 
    - its operations include +, -, *, /
- data types must match real world objects as closley as possible 
- user defined types
    - improves readability with meaningful names
    - improves modaifiability 
- uses of type system 
    - error detection with type checking 
    - program document info about its data
    