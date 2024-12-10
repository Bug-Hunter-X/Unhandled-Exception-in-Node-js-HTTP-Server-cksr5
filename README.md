# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications:  failure to handle exceptions properly in an HTTP server. The initial `bug.js` file lacks error handling, causing the server to crash unexpectedly if an error occurs.  The solution, `bugSolution.js`, demonstrates best practices for robust error handling.

## Bug Description
The `bug.js` code creates a simple HTTP server. However, it doesn't handle potential errors during request processing or server operations.  If an unexpected error happens, the server crashes without providing any useful information.

## Solution
The `bugSolution.js` file shows how to improve error handling by using `try...catch` blocks and `process.on('uncaughtException')` to gracefully handle errors.  Appropriate logging is added to provide debugging information.