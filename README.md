# Node.js EADDRINUSE Error
This repository demonstrates a common error in Node.js when starting an HTTP server on a port that's already in use.  The `bug.js` file shows the problematic code, and `bugSolution.js` provides a solution.

## Problem
Attempting to start an HTTP server on a port already occupied by another process results in an `EADDRINUSE` error. This often occurs during development when restarting a server quickly.

## Solution
The solution involves implementing proper error handling to gracefully deal with the `EADDRINUSE` error. This prevents crashes and allows the application to inform the user about the port conflict.