# descriptor 
- think of variable in terms of desriptors 
    - collection of attributes of a variable
    - area of memory that stores this 
        - static attributes: descriptors built and used at compile time 
        - dynamic: descritpor must be maintained during execution
    - used for type checing and code generation 

- one design issue is fundemental for all data types
    - what operations are provided for variables and how are they implimented 

# Primitive data types 
- almost all languages have them 
- are not defined in terms of other data types 
- some are merely reflections of the hardware 
- others require a little software support to impliment 

## int
- most int types supported directly by the hardware 
- many different int types 
    - byte (8 bits)
    - short (16 bits)
    - int (32 bits)
    - long (64 bits)
- python long int type not supported by hardware because they can get HUGE 
- some langs include unsigned ints (C++, C#)
    - are only positive 
- signed ints are strings of bits with the first one being a sign bit

## floats 
- model real numbers 
    - approximate
- pi cannont be represented as it is infinite 
    - nor can 0.1 (its represented as 0.0999755869...)
- langs for scientific purposes support at least 2 float types 
    - float and double
- represented by scientific notation where some bits are exponant and some bits are mantissa (fraction)
- float
    - 1 sign bit | 8 exponant bits | 23 fraction bits
- double 
    - 1 sign bit | 11 exponant bits | 52 fraction bits 
