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
    - EXECUTION PHASE
        - Runs the code line by line

Name/Value Pair: 
 - A name can be defined more than once, BUT can only have ONE value in any given context.
 - A value can be a collection of more name/value pairs.
Object:
 - Simply a collection of name/value pairs.

Undefined:
 - Special value meaning variable exists but has not been set.
 
JavaScript is SINGLE THREADED, SYNCHRONOUS (one line at a time) execution.

Execution Stack
 - Everytime a function is called, an execution context is created and pushed to the execution stack. 
 ![exStack](https://raw.githubusercontent.com/abidrahman/JS-Playground/master/Section-2/exstack.png)

Scope Chaining
 - Finding the definition of a variable that isn't defined in its own execution context.
 - A context's (eg. function's) OUTER ENVIRONMENT is dependent on its lexical environment.
 - Eg. If b() is called from within a() but physically sits in the global context, it has access to the global context's variables.

'let'
 - Cannot use a variable declared with 'let' until after where it is lexically declared.
 - Variable is available ONLY inside that block.

Async Callbacks
 - An Event Queue is filled by the browser.
 - When the execution context stack is empty, JS looks at the Event Queue and handles any waiting events.
 - Essentially still Synchronous.
```