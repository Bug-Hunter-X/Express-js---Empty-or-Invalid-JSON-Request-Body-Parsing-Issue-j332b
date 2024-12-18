# Express.js - Empty or Invalid JSON Request Body Parsing Issue

This repository demonstrates a common issue in Express.js applications where parsing an empty or invalid JSON request body leads to unexpected behavior. The `express.json()` middleware doesn't handle these cases appropriately by default.

## Bug Description
The provided code snippet demonstrates an Express.js application that attempts to parse a JSON request body.  However, if an empty request body or an invalid JSON string is sent, `req.body` remains empty, causing unexpected behavior or errors in the application logic.

## Solution
The solution involves using middleware to handle cases where the request body is empty or contains invalid JSON, potentially logging an error but ensuring consistent behavior and avoiding crashes.