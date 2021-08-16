# **Class 08**  

## **API Design Best Practices**  

>#### What does REST stand for?  

>>Answer,  
>>>Representational State Transfer.

>#### REST APIs are designed around a ____.

>>Answer,  
>>>REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client. 

>#### What is an identifer of a resource? Give an example.

>>Answer,    
>>>Focus on the business entities that the web API exposes. For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not. When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
>>>>https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest

>#### What are the most common HTTP verbs?

>>Answer,  
>>>Get, Post, Put, Patch, Delete

>#### What should the URIs be based on?

>>Answer,  
>>>REST APIs use Uniform Resource Identifiers (URIs) to address resources. On today’s web, URI designs range from masterpieces that clearly communicate the API’s resource model.
>>>>Guy Levin.

>#### Give an example of a good URI?

>>Answer,  
>>>URI = scheme "://" authority "/" path [ "?" query ] [ "#" fragment ]
>>>>Guy Levin.

>#### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

>>Answer,  
>>>Chatty API is one that requires consumers to make tremendous amount of distinct API calls to get needed information about a resource,  
No they are not a good thing because you are not being efficient with your API requests.

>#### What status code does a successful GET request return?

>>Answer,  
>>>200

>#### What status code does an unsuccessful GET request return?

>>Answer,  
>>>400

>#### What status code does a successful POST request return?

>>Answer,  
>>>200 or 204

>#### What status code does a successful DELETE request return?

>>Answer,  
>>>200 (ok), 202 (Accepted), 204 (No Content),

>#### How would you match your name using RegEx?

>>Answer,  
>>>
