# intro 
- imperitive languages based off of the Von neumann architecture 
    - efficiency is primary concern
- design of functional languages is based on math functions
    - a solid theoretical basis thats closer to the user but unconcerned with architecture 

# mathmatical functions 
- is a mapping of members of domain set onto range set 
- evaluation order of their mapping expresssions is controlled by recursion and conditional expressions 
    - rather than by squences and iteration 

# side effect 
- a function or expression has side effects if it modifies some state outside of its local scope 
- mathmatical functions have no side efffects and do not depend on any external values, they always map from domain to range in the same way every time 
# functional forms 
- a higher order fuctions, or functional form, is one that either takes functions as inputs, or yeilds functions as output, or both 
- it operates on other functions 
- one common kind of functional form is function composition 
## function composition
- combination of two functions to make a new fucntion
- h === f 0 g means h(x) === f( g( x ) )
- map is a built in function in may prog languages that takes a fucntion and a list as parameters, and applies the function to each element of the list 
# fundamentals of functional prog languages 
- the objective is to mimic mathmatical functions to the geatest extent possible 
- process of computation is fundementally different in FPGs
- a purely functional prog lang does not use variables or assignment statements 
- referential transparency: in FPLs, the result of a function is always the same given the same parameters 
- an FPL provides 
    - a set of primitive functions (+, -, *, /)
    - set of functional forms to construct complex functions 
    - function application operation 
    - structures for representing data 
# lisp 
- designed for easy manipulation of strings
- very old
- several dialects like common lisp and scheme 
- computation expressed as a funciton of at least one object 
- objects can be functions, data items, constants or variables, or data structures 
- ability to compute with symbolic expressions rather than numbers makes it good for AI
- Data objects: atoms and lists
- list form: parenthesized collections of sublists and/or atoms 
- lisp lists are stored internally as single-linked lists 
- functions are expressed the same way data is expressed 
- (A B C) could be a list A B C, or it could be the function A(B, C)
    - to distinguish data from functions, start data with apostrophe '(A B C)
- functions are specified in a prefix form 
    - (function parameter1 ... parametern)
- (+ 5 7) = 12
- (+ 3 4 7 6) = 20
- can display with (write((+ 5 7)))
# scheme 
- dialect of lisp 
- cleaner and more modern and simple 
- uses only static scoping 
- functions are first class entities 
    - they can be the values of expressions and elements of lists 
    - they can be assigned to variables, passed as parameters, and returned from functions
- literals evaluate to themselves 
- comments follow semicolons 
## primitive function evaluation
- the values of arguments are substituted into function body 
- function body evaluated
- the value of the last expression in the body is the value of the function 
- a nameless funciton includes the word lambda, adn is called a lambda expression 
- (lambda (x) (* x x)) returns the square of its given parameter
# defining functions
- simplest form 
    - (define symbol expression)
- (define pi 3.141593)
- (define two_pi (* 2 pi))
- control flow 
    - if 
    - (i predicate then_exp else_exp)
(if (> count 0)
    (/ sum count)
    (+ count 1)
)
- cond
(cont (test1
        (action1))
        (test 2
        (action2))
) and so on
- lists
- the list data type is a collection of ordered, non unique elements 
- part of functional languages 
- some imperative languages support lists too
- in lisp and scheme lists are enclosed in parentheses and use no punctuation 
- (A B C D)
- (A (B C) D)
- data and code have the same form 
- use apostrophe for data
- list operation
- car returns first element of its list parameter
- cdr returns a list, which is the remainder after first element is removed
- cons put its first parameter into its second parameter as a list to make a new list 
- list returns a new list of its paramenters