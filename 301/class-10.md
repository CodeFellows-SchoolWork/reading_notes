# **Class 10**  

## **Understanding the JavaScript Call Stack**  

>#### What is a ‘call’?

>>Answer,  
>>>The call stack is primarily used for function invocation (call).

>#### How many ‘calls’ can happen at once?

>>Answer,  
>>>One at a time,

>#### What does LIFO mean?

>>Answer,    
>>LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

>#### What causes a Stack Overflow?

>>Answer,    
>>A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## **JavaScript error messages**  

>#### What is a ‘refrence error’?

>>Answer,    
>>When you try to use a variable that is not yet declared you get this type os errors.

>#### What is a ‘syntax error’?

>>Answer,    
>>This occurs when you have something that cannot be parsed in terms of syntax.

>#### What is a ‘range error’?

>>Answer,    
>>Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

>#### What is a ‘tyep error’?

>>Answer,    
>>This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible.

>#### What is a breakpoint?

>>Answer,    
>>A breakpoint tels your code to stop at a specific point.

>#### What does the word ‘debugger’ do in your code?

>>Answer,    
>>The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

