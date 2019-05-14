# Lec Note - May 14

## Data Persistence

Use json array, to serialize the data.
Detelte, send the ID to the server and delete the object in the server.

## How to create User

return array then we can append the new user to the end of the array.
entry point of spingboot is in the main function.  
we can just run the application from the jar.  
  
If we just change the DOM, once refreshed, the changes will gone.  

Optimistic approach:
More details on the front end.  
Pessimatic approach:
More details on the back end.  

The more the information about other people, should be more pessimatic. Since we need to deal with concurrence or other situations.  

Send the userobject to the server. Any communication back to server is services. If it's user, it's user-services[CRUD about user] and if it's course it's course-services[CRUD about course].
All interaction is in the service folder.  
In JS the class is another function. Which is treated as a constructor.  
fetch() is vanlina JS which is like ajax in JQuery.  
Fetch() return a promise, notify browser when the data is ready. Promise could be an event to bed handled.  
The a in ajax is asyncinism. Promises allows us to syncalize all things together.  

## Implement in the sever side

```java
public List<User> createUser(@Requestbody User user){
    userArrayList.add(user);
    return suerArrayList;
}
```

## React!

jQuery is too low level. Fix the gap between anjuar 1 and 2.
Responsive for immdeiate feedback. Dynamically load the DOM, single page application. SPA.