---
author: aboude
---
# Operators
---

Created on: 2021-12-04-20:52
Last modified: 2022-01-20-10:11

---

### <span style="color: #ff5545">Arithmetic operators:</span>
| Key |      Name      | Use Example |   Result    |
|:---:|:--------------:|:-----------:|:-----------:|
|  +  |    addition    |    43+2     |     45      |
|  -  |  Subtraction   |    43-3     |     40      |
|  *  | Multiplication |     2*4     |      8      |
|  /  |    Division    |     4/2     |      2      |
|  %  |   Remainder    |    20%3     |      2      |
| ++  |   increment    |  x++ (x=2)  | x becomes 3 |
| --  |   Decrement    |  x-- (x=2)  | x becomes 1 |

### <span style="color: #ff5545">Assignment operators:</span>
| Key |          Name          | Use Example |    Same As     |
|:---:|:----------------------:|:-----------:|:--------------:|
|  =  |       Assignment       |    x = 5    |     x = 5      |
| +=  |       Add Assign       |   x += 5    |    x = x+5     |
| -=  |      Minus Assign      |   x -= 5    |    x = x-5     |
| *=  | Multiplication  Assign |   x *= 5    |    x = x*5     |
| /=  |    Division Assign     |   x /= 5    |    x = x/5     |
| %=  |    Remainder Assign    |   x %= 5    |    x = x%5     |
| &=  |       And Assign       |  x &= true  |  x = x & true  |
| \|= |       Or Assign        | x \|= false | x = x \| false |
| ^=  |       XOr Assign       |  x ^= true  |  x = x ^ true  |

### <span style="color: #ff5545">Relational Operators</span>
| Key |        Name        | Example | Result |
|:---:|:------------------:|:-------:|:------:|
| ==  |       Equals       | 5 == 5  |  true  |
| !=  |     Not Equals     | 4 != 5  |  true  |
|  >  |    Greater than    |  4 > 2  |  true  |
|  <  |     Less than      |  2 < 5  |  true  |
| >=  |  Greater or equal  | 2 >= 1  | false  |
| <=  | Less than or equal | 1 <= 5  |  true  |
### <span style="color: #ff5545">Logical operators</span>
| Key  | Name |     Example     | Result |
|:----:|:----:|:---------------:|:------:|
|  &&  | And  |  true && false  | false  |
| \|\| |  Or  | true \|\| false |  true  |
|  !   | Not  |      !true      | false  |
|  ^   | XOr  |  true ^ false   |  true  |

### <span style="color: #ff5545;text-transform: capitalize;">Unary, Binary, Ternary</span>

There exist another classification of operators, which devides operators on how many operands (5 + 6, `6` and `5` are operands and `+` is the operator) are used on an operator.

In the classification there exits three main types, `Unary`, `Binary` and `Ternary`

|     Uniary     |             Binary              |          Ternary          |
|:--------------:|:-------------------------------:|:-------------------------:|
| - (minus sign) | arithmatic operators (-,+,/,…)  | Conditional operator (?:) |
|    ! (not)     | Relational operators (<,=,>,>=) |                           |
|       ++       |     assignment (=, +=, -=)      |                           |
|       –-       |                                 |                           |

## Relevant:
[[Variable types]] | [[Variables]] | [[Booleans]]