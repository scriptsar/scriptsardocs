---
slug: promises-in-javascript
title: Promises In JavaScript
authors:
  name: Sarfaraz Hussain
  title: ScriptSar Core **Team**
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [webdev, JavaScript,Promise]
---

# What is Promise in Javascript

# Fundamentals of promise 
JavaScript, Promises are used to handle asynchronous operations, and they have three states: Pending, Fulfilled, and Rejected. Here's a detailed explanation of each state:

**Pending**: This is the initial state of a Promise. It means that the asynchronous operation hasn't completed yet, and the Promise is waiting for a result. When a Promise is in the Pending state, it can transition to either the Fulfilled or Rejected state, depending on the outcome of the asynchronous operation.

**Fulfilled**: This state means that the asynchronous operation was successful, and the Promise has resolved with a value. When a Promise is in the Fulfilled state, it means that the value that was promised is now available, and any then() callbacks attached to the Promise will be called with the resolved value.

**Rejected**: This state means that an error occurred during the asynchronous operation, and the Promise has been rejected with a reason (i.e., an error message or object). When a Promise is in the Rejected state, it means that the value that was promised cannot be delivered, and any `catch()` or `then()` callbacks that are attached to the Promise will be skipped until the error is handled.


```js
const promise = new Promise((resolve, reject) => {
  // Simulate an asynchronous operation that takes 3 seconds
  setTimeout(() => {
    const result = Math.random();

    if (result >= 0.5) {
      // Resolve the Promise with the result if it's greater than or equal to 0.5
      resolve(result);
    } else {
      // Reject the Promise with an error message if the result is less than 0.5
      reject(new Error('The result is less than 0.5'));
    }
  }, 3000);
});

promise.then((result) => {
  console.log('The Promise was fulfilled with the result:', result);
}).catch((error) => {
  console.error('The Promise was rejected with the error:', error);
});
```

# drawBacks if any