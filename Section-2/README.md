# Notes from Section 2
```
Syntax Parsers: A program that reads the code and determines what it does and if its grammar is valid.
Lexical Environment: Where something sits physically in the code and what surrounds it.
Execution Context: 
 - A wrapper that helps to manage the code that is running. Contains code that is running + more.
 - Creates a global object and 'this'.
 - The global object in a browser is the 'window' object.
 - Variables and functions get attached to global object when not in a scope.
 - Created in 2 phases
    - CREATION PHASE
        - Runs through code and recognizes variables/functions.
        - "Hoisting": Sets up memory space for vars/funcs.
            - Only stores variables, not their values, vars are set to undefined
            - All functions are stored in their entirety

Name/Value Pair: 
 - A name can be defined more than once, BUT can only have ONE value in any given context.
 - A value can be a collection of more name/value pairs.
Object:
 - Simply a collection of name/value pairs.
```