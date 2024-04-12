# First Node-js app

Node.js is an open-source, cross-platform JavaScript runtime environment that executes JavaScript code outside of a web browser. It allows developers to write server-side applications using JavaScript. Node.js is built on Chrome's V8 JavaScript engine and provides an event-driven architecture that enables asynchronous I/O operations, making it lightweight and efficient for building scalable network applications.

# Node.js vs. Browser JavaScript:

Environment:

Browser: Runs in a web browser, interacts with the DOM for webpage manipulation.
Node.js: Runs as a standalone application, enabling server-side programming and access to system resources.
APIs:

Browser: Provides DOM manipulation, event handling, AJAX requests, and browser-specific features.
Node.js: Offers APIs for file system operations, networking, HTTP server creation, and more, tailored for server-side development.
Access to Resources:

Browser: Limited access to system resources, confined within browser's security sandbox.
Node.js: Full access to system resources, allowing interaction with the file system, network, and operating system functionalities.



# Node.js CRUD App

This Node.js application demonstrates CRUD (Create, Read, Update, Delete) operations on a JSON file.

## Project Structure:


- `lib`: Contains server logic.
  - `handler.js`: Handles HTTP requests and CRUD operations.
- `server.js`: Sets up an HTTP server and uses `handler.js` for request handling.


## Requiring Files:

To require a file inside another file in Node.js, you use the `require` function. For example, let's say you want to use the functionalities from `handler.js` in `server.js`:

```javascript
// In server.js
const handler = require('./lib/handler');
```

Here, require('./lib/handler') imports the handler.js file located in the lib directory relative to server.js. The exported functionalities from handler.js can then be accessed using the handler variable within server.js.



## Tasks for the Student:

1. **Create Project Structure**:
   Create the project structure with the directory `lib` and the files `handler.js` and `server.js`. Provide brief descriptions for each file.

2. **Implement Data Handling**:
   In `handler.js`, handle HTTP requests sent from the form submission. Extract form data and implement CRUD (Create, Read, Update, Delete) operations on a JSON file. Here's how you can approach each operation:
   - **Create**: Parse the incoming request to extract data and add it to the JSON file.
   - **Read**: Retrieve data from the JSON file and send it as a response.
   - **Update**: Parse the incoming request to extract data and update the corresponding entry in the JSON file.
   - **Delete**: Parse the incoming request to identify the entry to be deleted and remove it from the JSON file.

3. **Update Server Configuration**:
   Modify `server.js` to import the `handler.js` module and use it to handle incoming requests.

4. **Test Implementation**:
   Ensure data is processed correctly and stored in the JSON file. Use tools like Thunder Client or Postman to send various types of requests (GET, POST, PUT, DELETE) to your server and verify that the CRUD operations work as intended.

Feel free to ask for clarification or assistance if needed!


