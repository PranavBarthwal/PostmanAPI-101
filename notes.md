###### Postman Academy Documentation : https://academy.postman.com/path/postman-api-fundamentals-student-expert/postman-api-fundamentals-student-expert-certification-1/1811

###### Postman Doc Link : https://letsupgrade.notion.site/Postman-Student-Expert-Certification-in-2-Days-fd88d22299b74158a05aaf8723504ee9 
<br>


# POSTMAN API FUNDAMENTALS
<br>

## UNDERSTANDING APIs 

### What is an API?
- API stands for **Application Programming Interface**.
- It's a way for different software applications to communicate with each other.

### Analogy: Restaurant Scenario
- **Customer**: Represents the user or client.
- **Waiter**: Acts as the API, facilitating communication between the customer and the kitchen.
- **Kitchen**: Corresponds to the backend service or server where the actual work occurs.

### Digital World Equivalence
- **Client**: You or your application.
- **API**: Acts as an intermediary, allowing your application to communicate with another application or service.
- **Backend System**: The other application or service where data processing, storage, or modification occurs.

### How APIs Work
- APIs define a set of **rules and protocols** for communication.
- They specify how different software components should **interact**, what **data** can be accessed or manipulated, and what **actions** can be performed.
- APIs enable developers to access specific features or functionalities of another application without understanding its internal workings.
- This fosters **interoperability** and facilitates the development of complex software systems by combining the capabilities of multiple components.

<br>


## Types of APIs



### Types of APIs based on Access, Medium, and Architecture

### 1. Access:

- **Open APIs (Public APIs)**:
   - These APIs are freely available to the public.
   - Designed for wide usage and accessibility.
   - Examples include social media APIs like Twitter, Facebook, etc.

- **Internal APIs (Private APIs)**:
   - Used within organizations for internal purposes.
   - Not exposed to the public.
   - Facilitate communication between internal systems or departments.

- **Partner APIs (B2B APIs)**:
   - Shared with trusted external partners or collaborators.
   - More restricted access compared to open APIs.
   - Used for sharing data and functionality with business partners.

### 2. Medium:

- **HTTP APIs**:
   - Utilize HTTP/HTTPS protocol for communication.
   - Commonly used for web-based APIs.
   - Examples include RESTful APIs and SOAP APIs.

- **WebSocket APIs**:
   - Enable bidirectional communication between client and server.
   - Suitable for real-time applications.
   - Used for applications requiring low latency and high concurrency.

- **GraphQL APIs**:
   - Allow clients to query only the data they need.
   - Provide a flexible and efficient approach to data retrieval.
   - Commonly used for building APIs that serve client-specific data requirements.

### 3. Architecture:

- **RESTful APIs**:
   - Follow the principles of Representational State Transfer (REST).
   - Stateless communication between client and server.
   - Use standard HTTP methods (GET, POST, PUT, DELETE).
   - Represent resources as URIs.
   - Examples include APIs for web services, e.g., Twitter API.

- **SOAP APIs**:
   - Based on the Simple Object Access Protocol (SOAP).
   - Use XML for message format.
   - Often used in enterprise environments.
   - Known for strong reliability and transactional support.

- **RPC APIs (Remote Procedure Call)**:
   - Allow clients to execute procedures or functions on remote servers.
   - Encapsulate function calls within network messages.
   - Examples include gRPC, XML-RPC.

- **Event-Driven APIs**:
   - Facilitate communication between components through events.
   - Decoupled architecture with event producers and consumers.
   - Suitable for asynchronous and loosely coupled systems.

These categorizations provide a comprehensive overview of different types of APIs based on their accessibility, communication medium, and architectural principles. The choice of API type depends on factors such as the specific use case, requirements, and constraints of the system being developed.

<br>

## POSTMAN

### Role of Postman in APIs

Postman is a popular tool used by developers to work with APIs. Its primary roles include:

1. **API Development**: Postman provides a platform for developers to design, build, and test APIs. Developers can create API endpoints, define request parameters, and set up response structures.

2. **API Testing**: It allows developers to send requests to APIs and analyze the responses. Postman offers a user-friendly interface for sending various types of requests such as GET, POST, PUT, DELETE, etc. Developers can also set up automated tests to ensure API functionality and performance.

3. **Documentation Generation**: Postman can automatically generate documentation for APIs based on the requests and responses configured within the tool. This documentation includes details such as endpoint URLs, request parameters, response formats, and examples.

4. **Collaboration**: Postman facilitates collaboration among team members working on API-related projects. Developers can share collections of requests, collaborate on API development and testing, and synchronize changes across team members.

5. **Monitoring and Debugging**: Postman allows developers to monitor API performance and debug issues. It provides insights into response times, error rates, and other metrics, helping developers identify and troubleshoot issues efficiently.

6. **Mock Servers**: Postman can create mock servers that simulate API behavior. This is useful during development and testing when the actual backend server may not be available or ready. Mock servers generate realistic responses based on predefined request-response pairs, enabling developers to test client applications effectively.

In summary, Postman plays a crucial role in the entire lifecycle of APIs, from development and testing to documentation and monitoring, making it an essential tool for API-centric development projects.

<br>

## cURL vs Postman

### cURL (Client for URLs)

1. **Command Line Tool**: cURL is a command-line tool used to transfer data using various network protocols, including HTTP, HTTPS, FTP, etc.
  
2. **Flexibility**: It provides a simple and flexible way to send HTTP requests with various options for customization.
  
3. **Automation**: cURL can be easily integrated into scripts and automated processes, making it suitable for tasks requiring command-line execution.
  
4. **Basic Features**: While powerful, cURL primarily offers basic functionalities such as sending requests, setting headers, and handling responses.
  
5. **Lack of GUI**: It lacks a graphical user interface (GUI), which may make it less user-friendly for some developers, especially those who prefer visual tools.

### Postman

1. **GUI Application**: Postman is a GUI-based application specifically designed for working with APIs.
  
2. **User-Friendly Interface**: It offers a user-friendly interface for building, testing, and debugging APIs, making it accessible to developers of all skill levels.
  
3. **Rich Feature Set**: Postman provides a wide range of features beyond basic request sending, including API documentation generation, automated testing, collaboration tools, monitoring, and mocking servers.
  
4. **Collections**: Postman allows developers to organize API requests into collections, making it easy to manage and share sets of requests with team members.
  
5. **Environment Variables**: It supports environment variables, allowing developers to define variables for dynamic data and streamline the testing process across different environments.
  
6. **Visual Debugging**: Postman offers visual debugging tools, making it easier to inspect request and response details, track variables, and troubleshoot issues.
  
7. **Integration with Third-Party Services**: Postman integrates with various third-party services and platforms, enhancing its capabilities for API development and testing.

#### Conclusion

- **cURL** is a powerful command-line tool suitable for quick and straightforward HTTP requests and automation tasks.
  
- **Postman** provides a comprehensive GUI-based platform tailored for API development, testing, documentation, and collaboration, offering a more robust and user-friendly experience for working with APIs.

<br>


## Request-Response Pattern in APIs

<img src="./Assets/Screenshot 2024-02-24 213752.png">


### 1. **Request Phase**:
   - **Client Sends Request**: The client, which could be a web browser, mobile application, or another server, sends a request to the API server. This request typically includes:
     - **Endpoint**: The specific URL or route that the client wants to access on the server.
     - **HTTP Method**: The type of action the client wants to perform, such as GET, POST, PUT, DELETE, etc.
     - **Headers**: Additional metadata or information accompanying the request, such as authentication tokens, content type, etc.
     - **Body (for some requests)**: Data sent to the server, usually for operations like creating or updating resources.

### 2. **Server Processing**:
   - **Routing**: The API server receives the request and routes it to the appropriate endpoint based on the URL and HTTP method specified in the request.
   - **Authentication & Authorization**: The server may authenticate the client's request to ensure it has the necessary permissions to access the requested resource.
   - **Data Processing**: The server processes the request, which may involve querying a database, performing calculations, or interacting with other services.
   - **Business Logic**: Any business rules or logic associated with the requested operation are executed.

### 3. **Response Phase**:
   - **Server Sends Response**: After processing the request, the server generates a response to send back to the client. This response typically includes:
     - **HTTP Status Code**: Indicates the outcome of the request (e.g., success, error, redirection, etc.).
     - **Headers**: Additional metadata accompanying the response, such as content type, caching directives, etc.
     - **Body (for most responses)**: Data sent back from the server to the client. This could be the requested resource, error messages, or other relevant information.

### 4. **Client Handling**:
   - **Response Parsing**: The client receives the response from the server and parses it to extract relevant data.
   - **Error Handling**: If the response indicates an error (e.g., 4xx or 5xx status code), the client may handle it accordingly, displaying error messages to the user or retrying the request.
   - **Data Display or Further Processing**: If the response is successful, the client may display the received data to the user, process it further, or take additional actions based on the response content.

### 5. **Optional Caching and Optimization**:
   - **Caching**: Both the client and server may utilize caching mechanisms to optimize performance by storing and reusing previously fetched data.
   - **Optimization Techniques**: Various optimization techniques such as compression, minification, and lazy loading may be employed to improve the efficiency of data transmission between the client and server.

### Conclusion:
The request-response pattern forms the backbone of communication between clients and servers in API-based systems. Understanding this pattern is crucial for building, consuming, and troubleshooting APIs effectively.

<br>

## Making a Request


To make a request, you typically need three essential ingredients:

1. **HTTP Method**:
   - The HTTP method specifies the type of action you want to perform on the server's resource. Common methods include:
     - **GET**: Retrieve data from the server.
     - **POST**: Submit data to the server to create a new resource.
     - **PUT**: Update an existing resource on the server.
     - **DELETE**: Remove a resource from the server.
     - And others like PATCH, HEAD, OPTIONS, etc.

    <img src="Assets/Screenshot 2024-02-24 203720.png">
    <img src="Assets/Screenshot 2024-02-24 204539.png">
    <img src="Assets/Screenshot 2024-02-24 204757.png">

2. **Address/Endpoint (URL)**:
   - The address or endpoint specifies the location of the resource on the server that you want to interact with. It's a unique identifier that the server uses to route your request to the appropriate handler. For example:
     ```
     https://api.example.com/resource
     ```

3. **Path**:
   - The path is a specific part of the URL that further specifies the location of the resource within the endpoint. It comes after the domain name and any optional parameters. For example, in the URL `https://api.example.com/users/123`, `/users/123` is the path, where `123` is a unique identifier for a specific user.

These three ingredients, combined together, provide the necessary information for the client to communicate with the server and perform the desired action on the resource.

<br>

## Status Codes

HTTP status codes are standardized responses that servers send back to clients (such as web browsers or API consumers) to indicate the success or failure of a request. Here's an overview of some common HTTP status codes:

### 1xx Informational
- **100 Continue**: The server has received the request headers and the client should proceed to send the request body.
- **101 Switching Protocols**: The server is switching protocols per the client's request.

### 2xx Success
- **200 OK**: The request was successful.
- **201 Created**: The request has been fulfilled, and a new resource has been created.
- **204 No Content**: The server successfully processed the request but is not returning any content.

### 3xx Redirection
- **301 Moved Permanently**: The requested resource has been permanently moved to a new location.
- **302 Found (Temporary Redirect)**: The requested resource has been temporarily moved to a different URI.
- **304 Not Modified**: Indicates that the resource has not been modified since the version specified by the request headers.

### 4xx Client Errors
- **400 Bad Request**: The server cannot process the request due to a client error, such as malformed syntax.
- **401 Unauthorized**: The request requires user authentication.
- **403 Forbidden**: The server understood the request but refuses to authorize it.
- **404 Not Found**: The server cannot find the requested resource.

### 5xx Server Errors
- **500 Internal Server Error**: A generic error message indicating that the server encountered an unexpected condition.
- **502 Bad Gateway**: The server received an invalid response from an upstream server while attempting to fulfill the request.
- **503 Service Unavailable**: The server is currently unable to handle the request due to temporary overload or maintenance.
- **504 Gateway Timeout**: The server, while acting as a gateway or proxy, did not receive a timely response from the upstream server.

These status codes provide a standardized way for servers to communicate the outcome of a request, allowing clients to understand and respond appropriately. Understanding these status codes is essential for troubleshooting issues when working with web services or APIs.