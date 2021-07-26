# **Class 03**  

## **React Docs - lists and keys**  

>#### What does .map() return?  

>>Answer,  
>>> it will return an array filled with X, where X= The value passed into .map() after it has been filtered by the corresponding code blocks.


>#### If I want to loop through an array and display each value in JSX, how do I do that in React? 

>>Answer,  
>>>We have an array filled with X,  
we now create a variable,  
I like to use const = Y,  
Y will now hold the return value of .map(),
X will be passed into .map() and it's return will be placed into an `<li>`{X}`<li>` making sure to use JSX syntax,  
We would then return `<ul>`{Y}`<ul>` because Y holds the return value of X after it has been procesed by .map() meaning Y holds the array of `<li>` that we wish to display.


>#### Each list item needs a unique ____.?  

>>Answer,    
>>> In React a unique 'KEY' is required as React uses the key value to keep track of what data has been processed. 

>#### What is the purpose of a key?

>>Answer,    
>>> In React the purpose of a key value is to keep track of the changes that have been made

## **The Spread Operator**  

>#### What is the spread operator?

>>Answer,  
>>>The spread operator is a tool that can be used to add X to an array, Combining arrays or objects and spreading an array out into a functions arguments by using a quick and easy syntax.

>#### List 4 things that the spread operator can do?

>>Answer,  
1. Adding to state in React,

1. Adding an item to a list, 

1. Copying an array,

1. Using an array as arguments

>#### Give an example of using the spread operator to combine two arrays?

>>Answer,  
>>> const xArr = [a,b,c],   
const yArr = [d,e,f],  
const zArr = [...xArr,...yArr],  
console.log(...zArr)

>#### Give an example of using the spread operator to add a new item to an array?

>>Answer, 
>>>const xArr = [1,2,3],  
const yArr = [4,5,6, ...xArr]
consol.log(yArr) //[4,5,6,1,2,3]

>#### Give an example of using the spread operator to combine two objects into one.?

>>Answer, 
>>>xObj = {A: "1"},  
yObj = {B: "2"},    
zObj = {...xObj, ...yObj, C: "3"}


## **How to Pass Functions Between Components**

>#### In the video, what is the first step that the developer does to pass functions between components?

>>Answer, 
>>>The first thing you must do is write the function in the place that the state lives above the render.

>#### In your own words, what does the increment function do?

>>Answer, 
>>>Increment is a function that takes in an object,  
The object contains a key value pair with (name) as the key,  
This function will create a NEW variable,  
We will call it X.  
the new const X = will contain the returned array from .map(),  
Y= the data that .map(Y) will process,  
It will then look at the Y object and see if it's name key === The (NAME) that was given as a prop,  
If Y === (NAME), the count of Y will increment by one and return.
Lastly we will this.setState({object: X});


>#### How can you pass a method from a parent component into a child component?

>>Answer, 
>>>Inside of the return object that is passing state down to a child,  
create a new variable that is passed in X={this.(methodName)}

>#### How does the child component invoke a method that was passed to it from a parent component?

>>Answer, 
>>>You find an acceptable place to put this.props(methodName(this.props.keyValuePair)) above the render(),  
In the return  on lets say an onClick={this.(method) that has access to this.props(methodName(this.props.keyValuePair)))}.

