# Bottom-Up-Parser-Implementation : Compiler-Construction

## Task-1:
- Write a program that can compute the first sets, for inputgrammar.
- Write a program that can compute the follow sets, for input grammar. 

- ### [Solution Task-1](https://github.com/hamzaiftkhar/Bottom-Up-Parser-Implementation-Compiler-Construction/tree/main/Question-1)

## Task-2:
- Write a program to create canonical collection of LR(0) items

- Write a program to implement the parsing table of LR(0) Parser

- Write a program to implement the parsing table of SLR(1) Parser

- ### [Solution Task-2](https://github.com/hamzaiftkhar/Bottom-Up-Parser-Implementation-Compiler-Construction/tree/main/Question-2)

## Task-3:

- Write a program to create canonical collection of LR(1) items

- Write a program to implement the parsing table of CLR(1) Parser

- Write a program to implement the parsing table of LALR(1) Parse

- ### [Solution Task-3](https://github.com/hamzaiftkhar/Bottom-Up-Parser-Implementation-Compiler-Construction/tree/main/Question-3%20(CLR%20and%20LALR))

## Task-4:

Show a complete LR(0) and SLR(1) parsers, including the canonical collection of LR(0) and parsing table, using the following grammar

```
E->E+T/T

T->TF/F

F->F*/a/b
```

Is this grammar LR(0) or SLR(1)? Why?
Verify your answers using the implementations of yours in Task 2. Attach a snippet of your results from your implementation.

- ### [Solution Task-4](https://github.com/hamzaiftkhar/Bottom-Up-Parser-Implementation-Compiler-Construction/tree/main/Question-4%20(LR0%20and%20SLR%20implementation))

## Task-5:

Construct CLR(1) and LALR(1) parsing table and parse the ababcstring following CLR(1) and LALR(1) parsing mechanism (if there are conflicts, point them out).

```
S->abABC/DE
A->a/epsilon
B->bA/epsilon
C->c
D->d/(E)
E->e/epsilon
```

Verify  your  answers  using  the  implementations of  yours  in  Task 3.  Attach a  snippet  of your resultsfrom your implementation.

### [Solution Task-5](https://github.com/hamzaiftkhar/Bottom-Up-Parser-Implementation-Compiler-Construction/tree/main/Question-5%20%20(CLR%20and%20LALR%20implementation))

## Contributions

- [Muhammad Hasnain - 21-CS-96  (Task-1,2)]()
- [Hamza Iftikhar - 21-CS-45   (Task-2,3,4)]()
- [Zunysha Naveed 21-CS-75   (Task-4,5)]()

University of Engineering and Technology Taxila

- [UET Taxila - Department of computer Science](https://www.uettaxila.edu.pk/)
- [Course : Compiler Construction]()
- [Course Instructor : DR ABID RAUF]()