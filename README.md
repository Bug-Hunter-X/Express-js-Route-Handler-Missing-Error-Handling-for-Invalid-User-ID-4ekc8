# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling for invalid input.  Specifically, the provided code attempts to parse a user ID from the request parameters as an integer without checking if the ID is a valid number. This can result in unexpected errors and crashes.

The `bug.js` file contains the erroneous code.  The `bugSolution.js` file provides a corrected version with robust error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express` to install the required dependency.
3. Run `node bug.js` and send a request to `/users/abc`. Observe the error.
4. Run `node bugSolution.js` and send a request to `/users/abc`. Observe the graceful error handling.