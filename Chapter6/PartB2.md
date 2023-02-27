## complex number
- expressed in the form `a + bi`
    - a and b are real numbers but i is the imaginary unit
        - i^2 = -1
    - some languages support complex types 
        - C99, Fortran, Python

## Decimal
- For buisness applications like money 
- stores a fixed number of decimal places 
- able to precisely store real numbers 
    - 0.1 can be exactly represented
- has limited range compared to floats and wastes memory 
- unpacked: each numeral is encoded into a single byte 
    - 91 = `0000 1001 0000 0001`
- packed: two numerals are encoded into a singe byte 
    - 91 = `1001 0001`
    - most significant bit is stored first 
    - sign is stored at the end 
    - decimal is fixed and not stored 

## boolean 
- simplest of all types 
    - true or false 
    - often implimented as bytes 

## char 
- stored as numeric coding 
    - ASCII table
        - uses 7 bits
        - stores 128 different chars
    - Unicode (UCS-2)
        - 16 bit
        - includes characters from most natrual langs
        - originally used in JAVA
        - C#, Python, Perl, JS also use it
    - 32 - bit Unicode (UCS-4)
        - Fortran

## Strings
- Values are sequesnces of chars 
    - ex `"john doe"`
- design issues 
    - is it a primitive or a special kind of char array?
    - should lenght be static or dynamic?
- typical operations 
    - assignment 
    - copying
    - comparison
    - catenation
    - substrings
    - pattern matching
- assignment and comparison are complicated 
    - beacuse they could be different lengths
    - in C, string assignments can bleed over into different strings!
- primitve or array?
    - in C/C++, strings are arrays
    - java and python: strings are literals
    - SNOBOL4
        - primitive 
        - many operation including pattern matching 
    - Fortran and Python
        - primitive 
        - immutable 
- pattern matching
    - use regular expressions 
    - character classes
        - [abc] - a, b, or c
        - [^abc] - any except a, b, or c
        - [a-zA-Z] - a through z or A through Z
        - [a-d[m-p]] - a through d or m through p
        - [a-z&&[def]] - d, e, or f (intersection of a-z and def)
        - [a-z&&[^bc]] - a through z besides b and c
        - [a-z&&[^m-p]] - a through z, minus m though p
        - /d - digit
    - Quantifiers 
        - X? - x occurs once or nor at all
        - X+ - X occurs one or more times
        - X* - X occurs zero or more times 
        - X{n} - X occurs n times only
        - X{n,} - X occurs n or more times
        - X{m,n} - X occurs m to n times 
    - examples 
        - /[A-Za-z][A-Za-z/d]+/
            - a letter followed by one or more letters and digits
        - /\d+\.?\d*|\.\d+/
            - Strings of one or more digits, possible followed by a decimal point, followed by zero or more digits
            - or strings that ebgin witha  decimal point, followed by one or more digits
            - basically a patter for written numbers 