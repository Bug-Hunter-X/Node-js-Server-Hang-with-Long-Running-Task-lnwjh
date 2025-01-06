# Node.js Server Hang with Long-Running Task

This repository demonstrates a common issue in Node.js where a long-running task in the request handler blocks the event loop, causing the server to hang.  The problem and a solution are provided.

## Problem

The `server.js` file contains a Node.js HTTP server that simulates a long-running task within the request handler. This blocks the event loop, preventing it from processing other requests.  As a result, the server becomes unresponsive.

## Solution

The `serverSolution.js` file demonstrates a solution using asynchronous operations to prevent blocking the event loop.  This allows the server to remain responsive even during long-running tasks.

## How to run

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `node server.js` to reproduce the bug.
4. Run `node serverSolution.js` to see the corrected version.