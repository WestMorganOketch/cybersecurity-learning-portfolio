Notes from my own practice on Hack The Box; not affiliated with or endorsed by Hack The Box.

# Web Requests and HTTP

This material explored how clients and servers communicate through HTTP requests and responses. The key skills were recognizing common request methods, understanding headers and response codes, and distinguishing request data from server responses. GET is commonly used to retrieve a representation, while POST commonly submits data for processing; APIs may also expose update and delete operations. The method alone does not determine whether an operation is safe or correctly authorized.

Important concepts include request lines, headers, content types, cookies, status codes, serialization, and CRUD-style API behavior. Testing should focus on expected behavior, input validation, authentication, authorization, and consistent error handling. Any test requests must remain within an approved lab or application scope.

From a defensive perspective, APIs should validate input on the server, enforce authorization for every object and operation, avoid exposing sensitive details in errors, use secure transport, and log security-relevant events without recording secrets. I would do differently by documenting expected request and response behavior before testing, checking authorization boundaries as well as functionality, and using sanitized examples in public notes.
