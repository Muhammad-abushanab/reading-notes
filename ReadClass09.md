## What are the five steps in the HTTP Request Lifecycle?

1. Local Processing.
2. Resolve IP Address.
3. Establish TCP Connection.
4. Send the HTTP Request.
5. Reslove and process the response.

## What are the two things the client needs before it can make an HTTP Request?

The client needs both the URL and DNS resolution before it can make an HTTP request. The URL specifies the destination of the request, and DNS resolution is necessary to obtain the IP address associated with the domain name in the UR

## Explain the four way handshake and what it does ?

1. (Client to Server) : The client initaites a process by sending a tcp segmant **FIN Flag** along with value **FIN-WAIT-1** which tells the Server he has finished sending data.
2. (Server to client) : Once reciveing the FIN segmant from the client the server start processing the acknowledgment  **ACK** to close the connection Along with value **CLOSE-WAIT**.
3. (Server to Client) : Once the server finishes sending data it starts to send his own **FIN** segmant along with the value **LAST-ACK**
4. (Client to server) : Once the client recieves the ack form the server he will respond with ack along with the value **TIME-WAIT** indicating that it has received the server's FIN segment

## True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer

Answer is True, This is due to the way HTTP redirects are used to indicate that a resource has moved to a different location or that the requested URL should be accessed through a different URL. Following redirects helps ensure that the client accesses the correct resource and maintains a smooth user experience. Failing to follow redirects could lead to broken links, outdated content, or security vulnerabilities.

## Which built-in Java class can be used to perform an HTTP request?

HttpURLConnection.

## What HTTP status codes represent a successful response? A redirect? A client error?

A Successful Responses (2xx):
**200 ok** : the request was successfull and server returned the data.

Redirection Responses (3xx):
**301 Moved Permanently** : The requested resource has been permanently moved to a different location. The client should update its bookmarks or links.

Client Error Responses (4xx):
**400 Bad Request** : Indicates that the client couldn't provide such as invalid paramter.

**403 Forbidden** : Indicates that the client has no access to this resource.

**404 NotFound** : which indicates that the requested url or data is not found.
