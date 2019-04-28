# Calculator Ver 1.03

Simple Console Calculator using C++ ver 1.03

[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://github.com/utilForever/CubbyCalc/blob/master/LICENSE) [![Build Status](https://travis-ci.org/utilForever/CubbyCalc.svg?branch=master)](https://travis-ci.org/utilForever/CubbyCalc/branches) [![Build status](https://ci.appveyor.com/api/projects/status/github/utilForever/CubbyCalc?branch=master&svg=true)](https://ci.appveyor.com/project/utilForever/CubbyCalc/branch/master) [![Build Status](https://dev.azure.com/utilforever/CubbyCalc/_apis/build/status/utilForever.CubbyCalc)](https://dev.azure.com/utilforever/CubbyCalc/_build/latest?definitionId=2)

## CodeMap

![CodeMap](https://github.com/utilForever/Calculator/blob/master/CodeMap.png)

## How to use

- ?: Help
- R: Read expression
- E: Evaluate and print latest expression
- E n: Evaluate and print nth expression
- P: Print latest expression postfix
- P n: Print nth expression postfix
- I: Print latest expression infix
- I n: Print nth expression infix
- T: Print latest expression tree
- T n: Print nth expression tree
- V: Print variable table list
- Q: Quit 

```
Calculator Version 1.02
?  : Help
R  : Read expression
E  : Evaluate and print latest expression
E n: Evaluate and print nth expression
P  : Print latest expression postfix
P n: Print nth expression postfix
I  : Print latest expression infix
I n: Print nth expression infix
T  : Print latest expression tree
T n: Print nth expression tree
V  : Print variable table list
Q  : Quit
>> R
a + b*s + c*sin(2*3.14*(d + t/e))
>> R
a=1
>> R
b=2
>> R
c=3
>> R
d=4
>> R
e=5
>> R
s=5
>> R
t=1.25
>> E 1
13.9997
```

## Version History

- Version 1.00

    - Implement binary operator (+, -, *, /, ^)
    - Implement unary operator (-)
    - Implement trigonometrical function (sin, cos, tan)
    - Implement expression tree (inheritance, polymorphism)
    - Implement infix to postfix converter
    - Implement variable table

- Version 1.01

    - Fix the bug (Recognize "sinx" as not "sin" + "x", but "sinx")
    
- Version 1.02
    
    - Constants refactoring (ExpressionMaker.cpp, ExpressionUtil.cpp → Constants.h)
    - Create help command
    
- Version 1.03

    - Enable to input multiple expressions (Separator: ",")     
        - Example     
        ```
        >> R
        a=1, b=2, c=3
        >> R
        a+b+c
        >> E
        6
        ```      
    - Remove friend class declaration (Calculator.h)
    - 1st ExpressionTree refactoring (UnaryOperator.h/cpp, BinaryOperator.h/cpp, Operand.h/cpp)    

## License

<img align="right" src="http://opensource.org/trademarks/opensource/OSI-Approved-License-100x137.png">

The class is licensed under the [MIT License](http://opensource.org/licenses/MIT):

Copyright &copy; 2015 [Chris Ohk](http://www.github.com/utiLForever)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
