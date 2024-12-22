# Express.js Route Handler Error: Missing parseInt() Error Handling

This repository demonstrates a common error in Express.js route handlers:  failure to handle cases where input data is not in the expected format.

The `bug.js` file contains the erroneous code, which attempts to parse a user ID from a route parameter using `parseInt()` without any error handling. If the user ID is not a number, `parseInt()` will return `NaN`, leading to unexpected behavior or crashes.

The corrected code is in `bugSolution.js`, which includes a check to ensure that the user ID is a valid number before attempting to parse it.  It also provides a proper 404 response if the user is not found.