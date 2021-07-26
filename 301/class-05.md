# **Class 05**  

## **React Docs - thinking in React**  

>#### How would you break a mock into a component heirarchy?  

>>Answer,  
>>>First thing i would do is examine the provided mock and break it down into single elements using the single responsibility principle that is commonly followed when coding components.


>#### What is the single responsibility principle and how does it apply to components? 

>>Answer,  
>>>This principle is simply to design each section of your code to only achieve one task,
When building a react app and specificity components each child component should only do one thing and if information is required to be used with other components then you should design your code to pass that information through the use of props.  



>#### What does it mean to build a ‘static’ version of your application?  

>>Answer,    
>>A static version is when you build the desired UI and component hierarchy limiting yourself to only using props to send data,  
This is done because once you have a static version built it becomes much easier and time effective to then start adding functionality.

>#### Once you have a static application, what do you need to add?

>>Answer,  
>>>The functionality of each component so this is where you may start to use your props and create state,

>#### What are the three questions you can ask to determine if something is state?

>>Answer,  
1. Is it passed in from a parent via props? If so, it probably isn’t state.  
1. Does it remain unchanged over time? If so, it probably isn’t state.  
1. Can you compute it based on any other state or props in your component? If so, it isn’t state.  

>#### How can you identify where state needs to live?

>>Answer,  
>>>Because of the one way flow nature of react when deciding where state should live you should examine what components need access to that state or is the state only accessed by one component,  
If the state is only handled by one component then it's usually safe to keep that state within the component, 
If multiple components need access to the state then your best bet is to find the parent that they all share and keep the state there.
