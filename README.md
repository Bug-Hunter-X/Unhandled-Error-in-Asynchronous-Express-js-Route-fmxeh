# Unhandled Error in Asynchronous Express.js Route

This repository demonstrates a common error in Node.js applications: unhandled errors within asynchronous operations.  The server crashes without proper error handling, leading to unexpected downtime.

## Bug Description:
The `bug.js` file contains an Express.js server with a route that simulates an asynchronous operation.  There's a 50% chance of an error being thrown, but this error isn't caught, leading to the server crashing.

## Solution:
The `bugSolution.js` file provides a corrected version with proper error handling. It uses a `try...catch` block to gracefully handle the potential error and send an appropriate response to the client.

## How to Reproduce the Bug:
1. Clone this repository.
2. Navigate to the directory containing `bug.js`.
3. Run `node bug.js`.
4. Refresh the page multiple times to observe the crash behavior (it might take a few attempts because of the 50% error probability).

## How to Run the Solution:
1. Navigate to the directory containing `bugSolution.js`.
2. Run `node bugSolution.js`.
3. Make requests to `http://localhost:3000` and observe the error handling mechanisms.
