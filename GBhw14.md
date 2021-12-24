HTTP Requests and Responses
Answer the following questions about the HTTP request and response process.


What type of architecture does the HTTP request and response process occur in?
Answer: Client-Server

What are the different parts of an HTTP request?
Answer: Request Line, header and body

Which part of an HTTP request is optional?
Answer: body

What are the three parts of an HTTP response?
Answer: Status Line, Headers and body

Which number class of status codes represents errors?
Answer: 400 and 500

What are the two most common request methods that a security professional will encounter?
Answer: GET and POST 

Which type of HTTP request method is used for sending data?
Answer: POST

Which part of an HTTP request contains the data being sent to the server?
Answer: Body

In which part of an HTTP response does the browser receive the web code to generate and style a web page?
Answer: Status Line -> Response Code

Using curl
Answer the following questions about curl:


What are the advantages of using curl over the browser?
Answer: You can transfer data from or to a server without user interaction. You can test web server security, Look for vulnerabilites on a web server 
and verify a server only respond to certain types of request.
Which curl option is used to change the request method?
Answer: -X  

Which curl option is used to set request headers?
Answer: --request

Which curl option is used to view the response header?
Answer: -I

Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?
Answer: options


Sessions and Cookies
Recall that HTTP servers need to be able to recognize clients from one another. They do this through sessions and cookies.
Answer the following questions about sessions and cookies:


Which response header sends a cookie to the client?
HTTP/1.1 200 OK
Content-type: text/html
Set-Cookie: cart=Bob
Answer: Set-Cookie

Which request header will continue the client's session?
GET /cart HTTP/1.1
Host: www.example.org
Cookie: cart=Bob
Answer: Connection Header -> HTTP/1.1


Example HTTP Requests and Responses
Look through the following example HTTP request and response and answer the following questions:
HTTP Request
POST /login.php HTTP/1.1
Host: example.com
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
Content-Type: application/x-www-form-urlencoded
Content-Length: 34
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Mobile Safari/537.36

username=Barbara&password=password


What is the request method?
Answer: POST

Which header expresses the client's preference for an encrypted response?
Answer: Accept-Encoding 

Does the request have a user session associated with it?
Answer: Yes 

What kind of data is being sent from this request body?
Answer: Application/x-www-form-urlencoded 

HTTP Response
HTTP/1.1 200 OK
Date: Mon, 16 Mar 2020 17:05:43 GMT
Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT
Content-Encoding: gzip
Expires: Fri, 01 May 2020 00:00:00 GMT
Server: Apache
Set-Cookie: SessionID=5
Content-Type: text/html; charset=UTF-8
Strict-Transport-Security: max-age=31536000; includeSubDomains
X-Content-Type: NoSniff
X-Frame-Options: DENY
X-XSS-Protection: 1; mode=block

[page content]


What is the response status code?
Answer: 200

What web server is handling this HTTP response?
Answer: Apache

Does this response have a user session associated to it?
Answer: Yes

What kind of content is likely to be in the [page content] response body?
Answer: Web page

If your class covered security headers, what security request headers have been included?
Answer: X-XSS-Protection


Monoliths and Microservices
Answer the following questions about monoliths and microservices:


What are the individual components of microservices called?
Answer: Clients, Identify and API Gateway

What is a service that writes to a database and communicates to other services?
Answer: SQL

What type of underlying technology allows for microservices to become scalable and have redundancy?
Answer: Docker


Deploying and Testing a Container Set
Answer the following questions about multi-container deployment:


What tool can be used to deploy multiple containers at once?
Answer: Docker Compose

What kind of file format is required for us to deploy a container set?
Answer: yaml


Databases


Which type of SQL query would we use to see all of the information within a table called customers?
Answer: SELECT * FROM customers 

Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)
Answer: INSERT INTO 

Why would we never run DELETE FROM <table-name>; by itself?
Answer: It deletes all the data in those fields whether its correct or not.




