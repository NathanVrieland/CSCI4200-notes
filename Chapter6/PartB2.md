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
