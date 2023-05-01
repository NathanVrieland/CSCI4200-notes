# BNF
- is identical to context free gammers
- like {assign} -> {var} = {expression}
- Terminal symbols are literals, like strings and ints
- nonterminal break down into terminals and other nontermianals
- Syntatctic lists are described using recursion
    - {ident_list} -> {ident} | {ident}, {ident_list}
# sentential form
- {program}
- begin {stmt_list} end
- begin {stmt}; {stmt_list} end
- begin a = b + c; b = {var} end
- begin a = B + c; b = c end
- a sentence is a setential form that only has terminal symbols 
- sentences are derived 