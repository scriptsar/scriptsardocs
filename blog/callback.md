---
slug: callback-function-in-javascript
title: Callback Function In JavaScript
authors:
  name: Sarfaraz Hussain
  title: ScriptSar Core **Team**
  url: https://github.com/wgao19
  image_url: https://avatars.githubusercontent.com/u/65873676?v=4
tags: [webdev, JavaScript,callback function]
---

# What is callback function 

 callback function is a function that is passed as an argument to another function and is called by that function when a certain event occurs or a certain task is completed. Callback functions are used to allow asynchronous programming, where a task is initiated, and the program continues to run while waiting for the task to complete.
A callback function is a function that is passed as an argument to another function and is executed or called back at some point inside the outer function. The purpose of a callback function is to allow code to be executed after an operation is completed, often asynchronously. The outer function that accepts the callback function as an argument can then invoke or call the callback function at an appropriate time, passing in any necessary parameters as arguments. This allows for greater flexibility and modularity in programming, as different callback functions can be used with the same outer function to achieve different results.
## synchronous Callback vs Aynchronous callback



# Why do we use callback function 


# How to use Callback function


# drabacks of callbacks

While callback functions are a powerful and widely used feature in JavaScript, they have some potential drawbacks that can make them hard to work with in certain situations. Here are some of the drawbacks of callback functions:

**Callback hell**: When using multiple nested callbacks, the code can quickly become hard to read and maintain, leading to a problem called "callback hell". 

```js
console.log('some code')
```
**Error handling**: When an error occurs in a callback function, it can be difficult to handle it properly, especially when there are multiple nested callbacks. Errors can also be easily missed or ignored, leading to unexpected behavior.
<!-- 
 For example: getData(function(data) { // ... }, function(error) { // ... });  -->

 **Lack of composition**: It can be difficult to compose and combine callback functions, especially when they have different argument and return types. This can make it hard to write modular and reusable code.

**Difficulty in managing asynchronous operations**: Callback functions can be difficult to use for managing complex asynchronous operations, such as handling multiple requests in parallel, chaining requests together, or handling errors and retries.
