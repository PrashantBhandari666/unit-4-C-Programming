# Operators and Expressions

## Operators
-------------------------------------
Operators are the foundation of any programming language. Thus the functionality of C programming language is incomplete without the use of operators. We can define operators as symbols that help us to perform specific mathematical and logical computations on operands. In other words, we can say that an operator operates the operands.

For example, consider the below statement:

```C
c = a + b;
```

Here, `` + ``  is the operator known as addition operator and ``a`` and ``b`` are operands. The addition operator tells the compiler to add both of the operands ``a`` and ``b``.

C language is rich in built-in operators and provides the following types of operators −

* Arithmetic Operator
* Relational Operator
* Logical Operator
* Assignment Operator
* Increment/decrement Operator
* Conditional Operator
* Bitwise Operator
* Comma Operator
* Sizeof Operator

### **Arithmetic Operator**
These are the operators used to perform arithmetic/mathematical operations on operands.

|Operator|       Meaning     | Example |
|:------:|-------------------|---------|
|    +   |      Addition     |  A + B  |
|    −   |    Subtraction    |  A − B  |
|    *   |  Multiplication   |  A * B  |
|    /   |      Division     |  B / A  |
|    %   |Modulus (remainder)|  B % A  |

### **Relational Operator**
These are used for comparison of the values of two operands. For example, checking if one operand is equal to the other operand or not, an operand is greater than the other operand or not etc.

|Operator|         Meaning            |Example|
|:------:|----------------------------|:-----:|
|   <    |is less than                |  a<b  |
|   <=   |is less than or equal to    | a<=b  |
|   >    |is greater than             |  a>b  |
|   >=   |is greater than or equal to | a>=b  |
|   ==   |is equal to                 | a==b  |
|   !=   |is not equal to             | a!=b  | 

### **Logical Operator**
Logical Operators are used to combine two or more conditions/constraints or to complement the evaluation of the original condition in consideration. The result of the operation of a logical operator is a boolean value either true or false.

|  Operator      |  Meaning                                               |   Example   |
|:--------------:|--------------------------------------------------------|:-----------:|
|  `&&`(AND)     |True only if both are True otherwise False              |   `a && b`  |
|  `∥`(OR)       |True if either of them are True ,False if all are false |   `a ∥ b`   |
|  `!`(AND)      |False if it is True,True if it is false                 |     `!a`    |
 
### **Assignment Operator**
Assignment operators are used to assign value to a variable. The left side operand of the assignment operator is a variable and right side operand of the assignment operator is a value. The value on the right side must be of the same data-type of variable on the left side otherwise the compiler will raise an error.

|Operator|         Meaning                                                                        |                    Example                      |
|:------:|----------------------------------------------------------------------------------------|:-----------------------------------------------:|
|   =    |Simple assignment operator. Assigns values from right side operands to left side operand|  ``a = 10;``                                    |
|   +=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a += b)`` can be written as ``(a = a + b)``  |
|   -=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a -= b)`` can be written as ``(a = a - b)``  |
|   *=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a *= b)`` can be written as ``(a = a * b)``  |
|   /=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a /= b)`` can be written as ``(a = a / b)``  |

### **Increment/decrement Operator** 
In C programming, the increment operator ``++`` increases the value of a variable by 1. Similarly, the decrement operator ``--`` decreases the value of a variable by 1.

### **Conditional Operator** 
The conditional operator is also known as a ternary operator. The conditional statements are the decision-making statements which depends upon the output of the expression. It is represented by two symbols, i.e., ``?`` and ``:``.

As conditional operator works on three operands, so it is also known as the ternary operator.

The behavior of the conditional operator is similar to the 'if-else' statement as 'if-else' statement is also a decision-making statement.

Syntax:
```c
variable = Expression1 ? Expression2 : Expression3  
```
It can be visualized into if-else statement as:  
```c
if(Expression1)
{
    variable = Expression2;
}
else
{
    variable = Expression3;
}
```
Example:
```c
x=(a>b)?a:b;
```
### **Bitwise Operator**
In arithmetic-logic unit (which is within the CPU), mathematical operations like: addition, subtraction, multiplication and division are done in bit-level. To perform bit-level operations in C programming, bitwise operators are used.

<table style="width:100%">
  <tr>
    <th>Operators</th>
    <th>Meaning of operators</th>
  </tr>
  <tr>
    <td>&</td>
    <td>Bitwise AND</td>
  </tr>
  <tr>
    <td>|</td>
    <td>Bitwise OR</td>
  </tr>
   <tr>
    <td>^</td>
    <td>Bitwise XOR</td>
  </tr>
  <tr>
    <td>~</td>
    <td>Bitwise complement</td>
  </tr>
   <tr>
    <td><<</td>
    <td>Shift left</td>
  </tr>
  <tr>
    <td>>></td>
    <td>Shift right</td>
  </tr>
</table>

### **Comma Operator**
The comma operator is a binary operator, that evaluates its first operand, and then discards the result, then evaluates the second operand and returns the value. The comma operator has the lowest precedence in C.

### **Sizeof Operator**
The sizeof operator is the most common operator in C. It is a compile-time unary operator and used to compute the size of its operand. It returns the size of a variable. It can be applied to any data type, float type, pointer type variables.

When ``sizeof()`` is used with the data types, it simply returns the amount of memory allocated to that data type. The output can be different on different machines like a 32-bit system can show different output while a 64-bit system can show different of same data types.

## Operator Precedence and Associativity
------------------------------------------------- 
### **Operator Precedence**
Operator precedence determines the grouping of terms in an expression and decides how an expression is evaluated. Certain operators have higher precedence than others; for example, the multiplication operator has a higher precedence than the addition operator.

For example, ``x = 7 + 3 * 2;`` here, ``x`` is assigned ``13``, not ``20`` because operator ``*`` has a higher precedence than ``+``, so it first gets multiplied with ``3*2`` and then adds into ``7``.

### **Associativity**
The associativity of operators determines the direction in which an expression is evaluated. For example,
```c
b = a;
```
Here, the value of ``a`` is assigned to ``b``, and not the other way around. It's because the associativity of the `` = `` operator is from right to left.

## Expressions and its Evaluation
-------------------------------------------------
An expression is a formula in which operands are linked to each other by the use of operators to compute a value. An operand can be a function reference, a variable, an array element or a constant.

```c
a - b;
```
>In the above expression, minus character (``-``) is an operator, and ``a``, and ``b`` are the two operands.

In the C programming language, an expression is evaluated based on the operator precedence and associativity. When there are multiple operators in an expression, they are evaluated according to their precedence and associativity. The operator with higher precedence is evaluated first and the operator with the least precedence is evaluated last.

>An expression is evaluated based on the precedence and associativity of the operators in that expression.

```
10 + 4 * 3 / 2
```
In the above expression, there are three operators ``+``, ``*`` and ``/``. Among these three operators, both multiplication and division have the same higher precedence and addition has lower precedence. So, according to the operator precedence both multiplication and division are evaluated first and then the addition is evaluated. As multiplication and division have the same precedence they are evaluated based on the associativity. Here, the associativity of multiplication and division is ``left`` to ``right``. So, multiplication is performed first, then division and finally addition. So, the above expression is evaluated in the order of ``*`` ``/`` and ``+``. It is evaluated as follows...

```
4 * 3 ====> 12

12 / 2 ===> 6

10 + 6 ===> 16
```
The expression is evaluated to 16.

## Type Casting in Expression
---------------------------------------------------
Type casting refers to changing an variable of one data type into another. The compiler will automatically change one type of data into another if it makes sense. For instance, if you assign an integer value to a floating-point variable, the compiler will convert the int to a float. Casting allows you to make this type conversion explicit, or to force it when it wouldn’t normally happen.

Type conversion in c can be classified into the following two types:

* Implicit Type Conversion
* Explicit Type Conversion

### **Implicit Type Conversion**
_When the type conversion is performed automatically by the compiler without programmers intervention, such type of conversion is known as implicit type conversion or type promotion._

_For example:_

```c
int x;
for(x=97; x<=122; x++)
{
    printf("%c", x);/*Implicit casting from int to char thanks to %c*/
}
```

### **Explicit Type Conversion**
_The type conversion performed by the programmer by posing the data type of the expression of specific type is known as explicit type conversion. The explicit type conversion is also known as type casting._

_Type casting in c is done in the following form:_

```c
(data_type)expression;
```
_where, ``data_type`` is any valid c data type, and ``expression`` may be constant, variable or expression._

_For example:_
```c
int x;
for(x=97; x<=122; x++)
{
    printf("%c", (char)x);/*Explicit casting from int to char*/
}
```
_The following rules have to be followed while converting the expression from one type to another to avoid the loss of information:_

* All integer types to be converted to float.
* All float types to be converted to double.
* All character types to be converted to integer.

## Program Statement:
------------------------
A computer program statement is an instruction for the computer program to perform an action. There are many different types of statements that can be given in a computer program in order to direct the actions the program performs or to control the order that the actions are carried out in.

### **Function**
_A program statement tells the computer to do something. This may be as simple as adding two numbers together or as complex as connecting to a server across the Internet._

### **Types**
_There are many types of program statements that you may find in a typical computer program. Assignment statements are used to assign a value to a program variable. Flow control statements help direct the order in which statements are performed. Iteration statements instruct the program to repeat a series of statements a specified number of times. These are just a few of the types of statements available to a programmer._

### **Considerations**
_There are many different programming languages, and each one has its own acceptable format for programming statements. A program statement that works fine in Java will not necessarily perform the same way in Visual Basic._
