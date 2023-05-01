# intro to parsing 
- why study lexical and syntax analysis 
    - apply grammars
    - compiler design
    - program listing formatters
    - programs that compute complexity of programs
    - programs that analyze and react the contents of a config file

- using BNF has 3 advantages 
    - makes syntax clear and consise
    - direct basis for syntax analyzers
    - is easy to maintain 

# analysis of syntax
- nearly all cmpilers sepearte the task of syntax analysis into 2 parts 
    - lexical analysis: turning lexemes into tokens 
    - syntax analysis or parsing: deals with large scale constructs 
- do this because 
    - simplicity
    - efficiency 
        - allows seperate optimisation 
    - portability 
        - parts of the lexical analyzer might not be portable, but the parser is

# lexical analysis 
- patter natcher for character strings
- it is a front end for the parser 
- turns lexemes into tokens 
- tokens are passed to the parser for santax analysis 

## three approaches 
- use regex 
    - write a formal discription of token patterns using regex
    - use this description as input for another tool to generate a lexical analyzer 
- state transition diagram 
    - describe token patterns and impliment diagram 
- table driven implimentation of the state transition diagram 

# state diagram 
- set of states 
- set of inputs 
- set of transitions
- example
    - start with get char
        - if starts with digit, transition to INT_LIT
            - take in any more digit input
        - if starts with letter, transition to IDENT
            - take in any more letter or didgit inputs
            