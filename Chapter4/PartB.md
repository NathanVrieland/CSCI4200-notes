# Syntax analysis 
## goals
- find syntax errors 
    - produce message and recover
- produce a parse tree
# parser
- categorized according to the direction they build parse trees 
    - top down 
        - produce parse tree beginning at the root
    - bottom up
        - begin at the leaves 
        - begin at the target string and try to arrive at the start symbol
- top down parser builds parse tree in preorder