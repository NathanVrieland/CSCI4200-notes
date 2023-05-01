# associativity of operators 
- plus and minus have the same precedence, but order still matters 
- need a rule called associativity 
- plus, minus, * and / are all evaluated left to right 
- they are left associative 
- they will be evaluated left to right 
- some operators, like exponents (** or ^) are evaluated right to left 
- so they are right associatve 
- the parser will parse the right most factors of exponents

# extended BNF
- optional parts in brackets []
    - {proc_call} -> ident [{expr_list}]
- repetitions are placed inside braces {}
    - {ident} -> letter {letter|digit}
- alternative parts are in paretheses and seperated with bars
    - {term} -> {term} (* | / | %) {factor}
