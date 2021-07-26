# **Class 04**  

## **React Docs - lists and keys**  

>#### What is a ‘Controlled Component’?  

>>Answer,  
>>> HTML elements such as `<input> <textarea>` and `<select>` usually maintain there own state and update it based on user input,  
In React however, state is usually kept in state property components and is only updated with setStste,  
So to make saving state happen smoothly in React we use methods to control the flow of state and only update it when we want the update to occur,


>#### Should we wait to store the users responses from the form into state when they submit the form? 

>>Answer,  
>>> setStat() automatically merges a partial state into current state, We only need to call it with the changed parts. 



>#### How do we target what the user is entering if we have an event handler on an input field?  

>>Answer,    
>>>You can add a name attribute to each element and let the handler function choose what to do based on th value of event.target.name

## **The Conditional (Ternary) Operator Explained**  

>#### Why would we use a ternary operator?

>>Answer,  
>>>Because it let's you write clean code when you are using true or false logic as it simplifies it into a one liner.

>#### Rewrite the following statement using a ternary statement?

>>Answer,  
>>>if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
>>>>> x === y ? console.log(true) : console.log(false);

