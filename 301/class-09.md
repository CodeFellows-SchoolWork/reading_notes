# **Class 09**  

## **Functional Programming Concepts**  

>#### What is functional programming?  

>>Answer,  
>>>Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia.

>#### What is a pure function and how do we know if something is a pure function?

>>Answer,  
>>>Pure Function is a function (a block of code ) that always returns the same result if the same arguments are passed. It does not depend on any state, or data change during a program’s execution rather it only depends on its input arguments.
>>>>geek5177


>#### What are the benefits of a pure function?

>>Answer,    
>>>One of the major benefits of using pure functions is they are immediately testable. They will always produce the same result if you pass in the same arguments.
They also makes maintaining and refactoring code much easier. You can change a pure function and not have to worry about unintended side effects messing up the entire application and ending up in debugging hell.
>>>>James Jeffery

>#### What is immutability?

>>Answer,  
>>>

>#### What is immutability?

>>Answer,  
>>>In JavaScript, only objects and arrays are mutable, not primitive values. ... A mutable object is an object whose state can be modified after it is created. Immutables are the objects whose state cannot be changed once the object is created.  
>>>>MDN

## **Node JS Tutorial for Beginners #6 - Modules and require()**  

>#### > What is a module?

>>Answer,  
>>>A module is like a component in react only on the server side,  
It is not a stand alone part of the code bace as modules are used to compartmentalize your code so that you can keep different parts of your code separated and only call upon the module and it's functions where they are required

>#### What does the word ‘require’ do?

>>Answer,  
>>>It's like importing and assigning the import to a variable in react only instead
of using the key word import we use require and assign it's value to a variable.

>#### How do we bring another module into the file the we are working in?

>>Answer,  
>>>require('./MODULE NAME')

>#### What do we have to do to make a module available?

>>Answer,  
>>>module.exports = FUNCTION NAME
