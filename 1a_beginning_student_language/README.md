# Notes on 1a Beginninng Student Language

## Module Overview
During this course the material will be taught in a programming languase called Beginning Student Language(BSL) it has been specifically design to be small simple, most of the language features can be learned in the first module. 

The simplicity creates the benifit of learning desing methods. BSL forms the core of nearly every other language that can be used through the life of a programmer. Using BSL means the design methods can be used on other programming languages.
**AVOID SKIMMING THROUGH THE MODULE.**
While BSL contains core of other programming languages it is different in important ways. Take your time to learn the material. 
### Learning Goals
- Write expressions that operate on primitive data which includes numbers, strings, images and booleans.
- Write constants and function definitions.
- Write out the step-by-step evaluation of simple expressionns which includes function calls.
- Use the stepper to automatically step through the evaluations of an expression.
- Use Dr Racket help desk to discover new primitives.


## Expressions
### Terms used:
- **Expression:** element of a program that is evaluated to produce a value.
- **Value:** data element such as 1(int), "foo"(stringn), (make-cat 10 20)(list)
- **Evaluate:** program executionns proceeds by evaluating expressionns to produce values.
- **Operator:** primitive operators are provided by language to operate on primitive data, this includes *,-,+, string-append, substring, image-width and many more.
- **Primitive:** Basic building block that is used to design a program. BSL containns primitive data and primitive operations.
- **Comment:** Comments is ignored bby BSL and it used to communicate to human reader something important or description of the program. A comment in BSL is create via ; and text followingn the ;.
- **Operand:** expression following the function name is a function call expression or operator name in a primitive call expression are called operands.
- **Argument:** value passed to a function or primitive operation when it is called. The arguments are values that result from evaluatinng the operands in the funnction or primitive call.  
- **Number:** primitive data that represent any number which include whole number, 0, fractions and decimals.

### Notes on Expressions, pt1
Top half of Dr Racket interface is called the definition area and bottom half is interation area. 
Definition area is used to design your program. Interation area is where your program output will go or the area you can interact with desinged program. 
Example of adition
The definition area contained
```racket
; the below is an expresion of primitives with operators
(+ 3 4)
``` 
Led to output in the interaction area:
```
; below is an evaluationn of the expression
7
```
More Complicated expression example input:
```racket
(+3 (* 2 3))
```
Output:
```
9
```
Form of a an expression in BSL is
```racket
(<primitive> <expression>...)
```
```...``` represents other expressions. 

To square a number use the primitive operation ```sqr```.
To square root a expressionn used ```sqrt```.
Example definition area for squaring:
```racket
(sqr 3)
```
Output interaction area:
```racket
9
```
Example definition area for square root:
```racket
(sqrt 16)
```
Output interaction area:
```
4
```
Excercise is file ```pythag-starter.rkt```
My working:
```racket
(sqrt (+ (sqr 3) (sqr 4)))
```
Output is ```5```
Which is correct.

### Note on Expressions, pt2:
What is means to be irrational numer is it takes infinite space to write the number down. Example of square rooting that will lead to irrational number.
```racket
(sqrt 2)
```
Lead to and output of:
```
#i1.4142135623730951
```
The i means it is an inexact number and the following number means it pretty close but not exactly.

## Evaluations
To understand big programs, we need to understand the detailed rules by which expressions get evaluated. We don't need to think of the rules but we can fall back on them.
## Strings and Images
## Constant Definitions
## Function Definitions
## Booleans and if Expressions
## Using the Stepper
## Discovering Primitives
## Practice Problems
## Module Wrap-up