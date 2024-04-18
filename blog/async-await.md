---
slug: async-await-in-javascript
title: Async Await In JavaScript
authors:
  name: Sarfaraz Hussain
  title: ScriptSar Core **Team**
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [webdev, JavaScript,async await]
---

# What is async wait

Async/await is a feature in JavaScript that allows you to write asynchronous code that looks and behaves like synchronous code. It was introduced in ES2017 and has quickly become a popular way to handle asynchronous operations in JavaScript.

Asynchronous code is code that doesn't run immediately, but instead, it runs in the background while other parts of the program continue to execute. The traditional way to handle asynchronous code in JavaScript is to use callbacks or promises, but async/await provides a more intuitive and readable syntax.

The async keyword is used to define a function that contains asynchronous code. The await keyword is used to pause the execution of a function until an asynchronous operation is completed. When the asynchronous operation is complete, the await keyword returns the result of the operation, allowing the function to continue executing.

Here is an example of how to use async/await to make an API call using the fetch function:

```js

async function getData() {
  const response = await fetch('https://api.example.com/data');
  const data = await response.json();
  console.log(data);
}

```


In this example, the fetch function returns a promise that resolves to a Response object. We use the await keyword to pause the execution of the function until the promise is resolved. We then call the json method on the Response object to get the data from the response, and again use the await keyword to pause the execution of the function until the data is retrieved.

Async/await makes it easier to write and understand asynchronous code in JavaScript, especially when dealing with complex, nested operations. However, it's important to remember that async/await only works with functions that return promises, and it's still important to handle errors appropriately