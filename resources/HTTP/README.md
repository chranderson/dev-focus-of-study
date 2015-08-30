#HTTP Protocol

## HTTP Codes & Meanings  
### 1xx Informational  
> This class of status code indicates a provisional response, consisting only of the Status-Line and optional headers, and is terminated by an empty line. Since HTTP/1.0 did not define any 1xx status codes, servers must not[note 1] send a 1xx response to an HTTP/1.0 client except under experimental conditions.  

[**100** Continue](#100-continue)  
[**101** Switching Protocols](#101-switching-protocols)  
[**102** Processing](#102-processing)  

### 2xx Success  
> This class of status codes indicates the action requested by the client was received, understood, accepted and processed successfully.  

[**200** OK](#200-ok)  
[**201** Created](#201-created)  
[**202** Accepted](#202-accepted)  
[**203** Non-Authoritative Information (since HTTP/1.1](#203-non-authoitative-information)  
[**204** No Content](#204-no-content) 
[**205** Reset Content](#205-reset-content)  
[**206** Partial Content](#206-partial-content)  
[**207** Multi-Status](#207-multi-status)  
[**208** Already Reported](#208-already-reported)  
[**226** IM Used (RFC 3229)](#im-used)  


## 3xx Redirection  
> This class of status code indicates the client must take additional action to complete the request. Many of these status codes are used in URL redirection.  
A user agent may carry out the additional action with no user interaction only if the method used in the second request is GET or HEAD. A user agent should not automatically redirect a request more than five times, since such redirections usually indicate an infinite loop.  

[**300** Multiple Choices](#300-multiple-choices)  
[**301** Moved Permanently](#301-moved-permanently)  
[**302** Found](#302-found)  
[**303** See Other](#303-see-other) (since HTTP/1.1)  
[**304** Not Modified](#304-not-modified) (RFC 7232)  
[**305** Use Proxy](#305-use-proxy) (since HTTP/1.1)   
[**306** Switch Proxy](#306-switch-proxy)  
[**307** Temporary Redirect](#307-temporary-redirect) (since HTTP/1.1)   
[**308** Permanent Redirect](#308-permanent-redirect) (RFC 7538)  
[**308** Resume Incomplete](#308-permanent-redirect) (Google)  





***  

#### 100 Continue
> This means that the server has received the request headers, and that the client should proceed to send the request body (in the case of a request for which a body needs to be sent; for example, a POST request). If the request body is large, sending it to a server when a request has already been rejected based upon inappropriate headers is inefficient. To have a server check if the request could be accepted based on the request's headers alone, a client must send Expect: 100-continue as a header in its initial request and check if a 100 Continue status code is received in response before continuing (or receive 417 Expectation Failed and not continue).


#### 101 Switching Protocols
> This means the requester has asked the server to switch protocols and the server is acknowledging that it will do so.


#### 102 Processing
> As a WebDAV request may contain many sub-requests involving file operations, it may take a long time to complete the request. This code indicates that the server has received and is processing the request, but no response is available yet.[3] This prevents the client from timing out and assuming the request was lost.

  
#### 200 OK  
> Standard response for successful HTTP requests. The actual response will depend on the request method used. In a GET request, the response will contain an entity corresponding to the requested resource. In a POST request, the response will contain an entity describing or containing the result of the action.  

#### 201 Created  
> The request has been fulfilled and resulted in a new resource being created.  

#### 202 Accepted  
> The request has been accepted for processing, but the processing has not been completed. The request might or might not eventually be acted upon, as it might be disallowed when processing actually takes place.   

#### 203 Non-Authoritative Information (since HTTP/1.1)  
> The server successfully processed the request, but is returning information that may be from another source.  

#### 204 No Content    
> The server successfully processed the request, but is not returning any content.  

#### 205 Reset Content  
> The server successfully processed the request, but is not returning any content. Unlike a 204 response, this response requires that the requester reset the document view.  

#### 206 Partial Content  
> The server is delivering only part of the resource (byte serving) due to a range header sent by the client. The range header is used by tools like wget to enable resuming of interrupted downloads, or split a download into multiple simultaneous streams.  

#### 207 Multi-Status  
> The message body that follows is an XML message and can contain a number of separate response codes, depending on how many sub-requests were made.  

#### 208 Already Reported    
> The members of a DAV binding have already been enumerated in a previous reply to this request, and are not being included again.  

#### 226 IM Used (RFC 3229)   
> The server has fulfilled a request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.  


#### 300 Multiple Choices    
> Indicates multiple options for the resource that the client may follow. It, for instance, could be used to present different format options for video, list files with different extensions, or word sense disambiguation.  

#### 301 Moved Permanently     
> This and all future requests should be directed to the given URI.  

#### 302 Found       
> This is an example of industry practice contradicting the standard. The HTTP/1.0 specification (RFC 1945) required the client to perform a temporary redirect (the original describing phrase was "Moved Temporarily"),[6] but popular browsers implemented 302 with the functionality of a 303 See Other. Therefore, HTTP/1.1 added status codes 303 and 307 to distinguish between the two behaviours.[7] However, some Web applications and frameworks use the 302 status code as if it were the 303.  

#### 303 See Other (since HTTP/1.1)         
> The response to the request can be found under another URI using a GET method. When received in response to a POST (or PUT/DELETE), it should be assumed that the server has received the data and the redirect should be issued with a separate GET message.    

#### 304 Not Modified (RFC 7232)         
> Indicates that the resource has not been modified since the version specified by the request headers If-Modified-Since or If-None-Match. This means that there is no need to retransmit the resource, since the client still has a previously-downloaded copy.  

#### 305 Use Proxy (since HTTP/1.1)         
> The requested resource is only available through a proxy, whose address is provided in the response. Many HTTP clients (such as Mozilla and Internet Explorer) do not correctly handle responses with this status code, primarily for security reasons.  

#### 306 Switch Proxy     
> No longer used. Originally meant "Subsequent requests should use the specified proxy."    

#### 307 Temporary Redirect (since HTTP/1.1)       
> In this case, the request should be repeated with another URI; however, future requests should still use the original URI. In contrast to how 302 was historically implemented, the request method is not allowed to be changed when reissuing the original request. For instance, a POST request should be repeated using another POST request.      
#### 308 Permanent Redirect (RFC 7538)    
> The request, and all future requests should be repeated using another URI. 307 and 308 (as proposed) parallel the behaviours of 302 and 301, but do not allow the HTTP method to change. So, for example, submitting a form to a permanently redirected resource may continue smoothly.  

#### 308 Resume Incomplete (Google)  
> This code is used in the Resumable HTTP Requests Proposal to resume aborted PUT or POST requests.  


#### 400 Title  
> text here.  

  
#### 500 Title  
> text here.  


