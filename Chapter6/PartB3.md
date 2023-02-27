## more strings 
- static length 
    - length is set when string is created
- limited dynamic length 
    - strings can store any number of chars between zero and a fixed maximum set at variables definition 
        - C: `char s[50] = "abcde";`
- Dynamic length 
    - allow strings to have varying length with no max
    - fexibile
    - more overhead 

## string evaluation
- strings aid writability
- strings as arrays can be cumbersome compared to strings as primitives 
- providing them through a standard library is nearly as convinient as having primitive type 
- static lenth strings need compile time desctiptors 
- limited dynamic length strings may need run time descriptor 
    - c and c++ strings do not because they end in a null character 
- dynamic length strings need a runtime descriptor 
- three approaches to dynamic length strings 
    - strings stored as linked list of characters 
    - store strings as an array of pointers to chars
        - uses extra memory, but is faster 
    - store complete strings in adjacent memory cells 
        - when string grows, the entire string might need to be moved 
    