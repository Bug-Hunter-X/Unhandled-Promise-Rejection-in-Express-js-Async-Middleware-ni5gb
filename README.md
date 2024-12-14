# Unhandled Promise Rejection in Express.js Async Middleware

This repository demonstrates a common error in Express.js applications: unhandled promise rejections in asynchronous middleware.  The `bug.js` file shows the flawed code, while `bugSolution.js` provides a corrected version.  Failing to properly handle errors within asynchronous operations can lead to application crashes and unexpected behavior.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Observe the server crashing without a proper error message.

## Solution

The solution involves using `.catch()` to handle any rejected promises within the asynchronous operation, ensuring the server does not crash. See `bugSolution.js` for the corrected code.