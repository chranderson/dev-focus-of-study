#HTTP Protocol

## HTTP Codes & Meanings
[**100** Continue](#100-continue)
[**101** Switching Protocols](#switching-protocols)
[**102** Processing](#processing)

***

### **100** Continue
> This means that the server has received the request headers, and that the client should proceed to send the request body (in the case of a request for which a body needs to be sent; for example, a POST request). If the request body is large, sending it to a server when a request has already been rejected based upon inappropriate headers is inefficient. To have a server check if the request could be accepted based on the request's headers alone, a client must send Expect: 100-continue as a header in its initial request and check if a 100 Continue status code is received in response before continuing (or receive 417 Expectation Failed and not continue).


### **101** Switching Protocols
> This means the requester has asked the server to switch protocols and the server is acknowledging that it will do so.


### **102** Processing
> As a WebDAV request may contain many sub-requests involving file operations, it may take a long time to complete the request. This code indicates that the server has received and is processing the request, but no response is available yet.[3] This prevents the client from timing out and assuming the request was lost.

