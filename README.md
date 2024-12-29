# Web-Development
Homework 14

Overview:

In this homework, we will review the many of the concepts and tools covered in the Web Development unit.

Questions
Before you work through the questions below, please create a new file and record your answers there. This will be your homework deliverable.

HTTP Requests and Responses Answer the following questions about the HTTP request and response process.

1) What type of architecture does the HTTP request and response process occur in?

Answer
Client server architecture. Requests are made from client to server then back to client.

2) What are the different parts of an HTTP request?

Answer
Request Line, Request Headers, Request Body

3) Which part of an HTTP request is optional?

Answer
Request Body

4) What are the three parts of an HTTP response?

Answer
Headers, Status Line, Body

5) Which number class of status codes represents errors?

Answer
[400..499] :: Client errors && [500..599] :: Server errors

6) What are the two most common request methods that a security professional will encounter?

Answer
Post, & get.

7) Which type of HTTP request method is used for sending data?

Answer
POST Request

8) Which part of an HTTP request contains the data being sent to the server?

Answer
Request body

9) In which part of an HTTP response does the browser receive the web code to generate and style a web page?

Answer
Response body
Using curl

10) What are the advantages of using curl over the browser?

Answer
manage the HTTP Requests / Responses in a Repeatable , Programmatic way
also quickly test HTTP HTTP Requests in away that can be automated
Allows to make the adjustments as the security professional works
And it support numerous protocols even if a UI is not present

11) Which curl option is used to change the request method?

Answer
Curl -X

12) Which curl option is used to set request headers?

Answer
Curl -H

13) Which curl option is used to view the response header?

Answer
Curl -i

14) Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?

Answer
Get
Sessions and Cookies
Recall that HTTP servers need to be able to recognize clients from one another. They do this through sessions and cookies.

15) Which response header sends a cookie to the client? HTTP/1.1 200 OK Content-type: text/html Set-Cookie: cart=Bob

Answer
Set-Cookie sends cookie to client

16) Which request header will continue the client's session? GET /cart HTTP/1.1 Host: www.example.org Cookie: cart=Bob

Answer
Cookie will save/continue the client's

Example HTTP Requests and Responses:

Look through the following example HTTP request and response and answer the following questions: HTTP Request POST /login.php HTTP/1.1 Host: example.com Accept-Encoding: gzip, deflate, br Connection: keep-alive Content-Type: application/x-www-form-urlencoded Content-Length: 34 Upgrade-Insecure-Requests: 1 User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Mobile Safari/537.36

username=Barbara&password=password

17) What is the request method?

Answer
POST

18) Which header expresses the client's preference for an encrypted response?

Answer
Upgrade-insecure-requests 1

19) Does the request have a user session associated with it?

Answer
The Session is not restablished yet, so No

20) What kind of data is being sent from this request body?

Answer
Login credentials
HTTP Response HTTP/1.1 200 OK Date: Mon, 16 Mar 2020 17:05:43 GMT Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT Content-Encoding: gzip Expires: Fri, 01 May 2020 00:00:00 GMT Server: Apache Set-Cookie: SessionID=5 Content-Type: text/html; charset=UTF-8 Strict-Transport-Security: max-age=31536000; includeSubDomains X-Content-Type: NoSniff X-Frame-Options: DENY X-XSS-Protection: 1; mode=block


21) What is the response status code?

Answer
cc

22) What web server is handling this HTTP response?

Answer
Apache webserver

23) Does this response have a user session associated to it?

Answer
Yes SessionID=5

24) What kind of content is likely to be in the [page content] response body?

Answer
Detail of the page configuration

25) If your class covered security headers, what security request headers have been included?

Answer
Strict transport security, or XSS protection.
Monoliths and Microservices

26) What are the individual components of microservices called?

Answer
Services

27) What is a service that writes to a database and communicates to other services?

Answer
APIs

28) What type of underlying technology allows for microservices to become scalable and have redundancy?

Answer
Load Plancer OR Containers
Deploying and Testing a Container Set

29) What tool can be used to deploy multiple containers at once?

Answer
Docker

30) What kind of file format is required for us to deploy a container set?
Answer
.yml Yaml format
Databases

31) Which type of SQL query would we use to see all of the information within a table called customers?

Answer
Select Column & From Customers.

32) Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)

Answer
INSERT INTO [columns] VALUES [values]

33) Why would we never run DELETE FROM ; by itself?

Answer
It will delete the entire table there is no select stateme
