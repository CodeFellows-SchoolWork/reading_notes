# **Class 02**  

## **React Lifecycle**  

>### **Question- what happens first?**  

>>#### ‘render’ or ‘componentDidMount’?  

>>>Answer,  
Before the componentDidMount happens the render will occurred first as this is the lifecycle of react.  

>### **Question ? What is the first thing to occur in the lifecycle of React?**  

>>Answer,  
We start by Mounting and enter into the constructor which is the start of the render phase.  

>### **Question ? Put the following things in the order that they happen:**  

* `componentDidMount`  

* `render`  

* `constructor`

* `componentWillUnmount`  

* `React Updates`  

1. `constructor`

1. `render`  

1. `componentDidMount`  

1. `React Updates`  

1. `componentWillUnmount`  

## **React State Vs Props**  

>#### **What types of things can you pass in the props?**  

>>Answer,  
>>> You would use props to pass in data that a component needs in order to complete the desired action,  
This could be a string such as a `<h1>` or any other properties you would give a basic function.

>#### **What is the big difference between props and state?**

>>Answer,  
>>>You can pass in a prop to a component but this prop cannot be changed because the prop is handled outside of the component (this is a good example of react one way flow in action),  
State on the other hand is handled inside of the component and is able to be changed or updated if required from within the component.


>#### **When do we re-render our application?**

>>Answer,  
>>>Anytime a component or it's state changes,  
The react app will re-render.

>#### **What are some examples of things that we could store in state?**

>>Answer,  
>>>We could use state keep track of user inputs,  
Maybe we have a counter assigned to a button and want to keep track of it's clicks,
Or Maybe we want to get the users name and send that as a prop to be used in another component.  


