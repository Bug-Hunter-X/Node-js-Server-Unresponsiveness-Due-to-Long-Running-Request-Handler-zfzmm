# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js applications: server unresponsiveness caused by long-running operations within request handlers.  A simple HTTP server is created that simulates a long-running task (5-second delay).  During this delay, the server cannot handle other requests, potentially leading to timeouts or connection issues for clients.

The `bug.js` file contains the problematic code.  The `bugSolution.js` file provides a solution using asynchronous operations and event loops to prevent blocking.