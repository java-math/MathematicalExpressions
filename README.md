#Java Library to Evaluate String Mathematical Expressions

This is a smiple Java library that can be used to solve mathematical expressions. You can input your mathematical expressions as a string variable and this library convert them to mathematical expressions and solves them.

For bad expressions that can't be solved, the library will throw

```java
src.com.achinthagunasekara.mathematical.BadMathematicalExpressionException
```

##Import the library into your Java application

```Java
import com.achinthagunasekara.mathematical.MathExpressions;
```

You can create a new instance of MathExpressions object by

```java
MathExpressions me = new MathExpressions();
```

## Calculations

To evaluate a string mathematical expression,

```java
System.out.println(me.evaluate("3*4"));
System.out.println(me.evaluate("4+5"));
```

##History

To get a history of previous mathematical expressions,

```java
me.getHistory(); //returns a ArrayList<String> with past expressions
```

You can also get a specific past expression by entering a expression number

```java
me.getHistory(3); //returns a String with # 3 expression
```

To clear history,

```java
me.clearHistory(); //clear all past expressions in the history
```

##Printing

To print history of input mathematical expressions,

```java
printHistory(); //prints history on screen
```

To print history and solutions to input mathematical expressions

```java
printHistoryAndSolutions(); //prints history and solutuins on screen
```

Above function is a overloaded function. You can call it with a boolean parameter called printFullErrors
