# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers:  failure to handle cases where input parameters are invalid or missing.  Specifically, this example shows a route that fetches a user by ID, but lacks proper error handling if the ID is not a valid integer.

## Bug

The `bug.js` file contains an Express.js route handler that attempts to fetch a user from an array based on the ID passed in the request parameters.  However, it doesn't check if the ID is a valid number before attempting to parse it as an integer. This leads to a potential error if a non-numeric ID is provided. 

## Solution

The `bugSolution.js` file provides a corrected version of the route handler that includes error handling to catch and gracefully handle non-numeric IDs.