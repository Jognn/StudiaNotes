## Extern C 

- Powoduje, że kompilator C++ użyje linkage C (bez name manglingu)

""" 
In every C++ program, all non-static functions are represented in the binary file as symbols. These symbols are special text strings that uniquely identify a function in the program.

In C, the symbol name is the same as the function name. This is possible because in C no two non-static functions can have the same name.

Because C++ allows overloading and has many features that C does not — like classes, member functions, exception specifications - it is not possible to simply use the function name as the symbol name. To solve that, C++ uses so-called name mangling, which transforms the function name and all the necessary information (like the number and size of the arguments) into some weird-looking string processed only by the compiler and linker.

So if you specify a function to be extern C, the compiler doesn't performs name mangling with it and it can be directly accessed using its symbol name as the function name.

This comes handy while using `dlsym()` and `dlopen()` for calling such functions.
""""


LINK - https://stackoverflow.com/questions/1041866/what-is-the-effect-of-extern-c-in-c
https://stackoverflow.com/questions/13694605/how-to-use-c-source-files-in-a-c-project/51912672#51912672