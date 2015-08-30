#HTTP Protocol

## HTTP Codes & Meanings  
### 1xx Informational  
> This class of status code indicates a provisional response, consisting only of the Status-Line and optional headers, and is terminated by an empty line. Since HTTP/1.0 did not define any 1xx status codes, servers must not[note 1] send a 1xx response to an HTTP/1.0 client except under experimental conditions.  

> [**100** Continue](#100-continue)  
> [**101** Switching Protocols](#101-switching-protocols)  
> [**102** Processing](#102-processing)  

### 2xx Success  
> This class of status codes indicates the action requested by the client was received, understood, accepted and processed successfully.  

> [**200** OK](#200-ok)  
> [**201** Created](#201-created)  
> [**202** Accepted](#202-accepted)  
> [**203** Non-Authoritative Information (since HTTP/1.1](#203-non-authoitative-information)  
> [**204** No Content](#204-no-content) 
> [**205** Reset Content](#205-reset-content)  
> [**206** Partial Content](#206-partial-content)  
> [**207** Multi-Status](#207-multi-status)  
> [**208** Already Reported](#208-already-reported)  
> [**226** IM Used (RFC 3229)](#im-used)  


## 3xx Redirection  
> This class of status code indicates the client must take additional action to complete the request. Many of these status codes are used in URL redirection.  
A user agent may carry out the additional action with no user interaction only if the method used in the second request is GET or HEAD. A user agent should not automatically redirect a request more than five times, since such redirections usually indicate an infinite loop.  

> [**300** Multiple Choices](#300-multiple-choices)  
> [**301** Moved Permanently](#301-moved-permanently)  
> [**302** Found](#302-found)  
> [**303** See Other](#303-see-other) (since HTTP/1.1)  
> [**304** Not Modified](#304-not-modified) (RFC 7232)  
> [**305** Use Proxy](#305-use-proxy) (since HTTP/1.1)   
> [**306** Switch Proxy](#306-switch-proxy)  
> [**307** Temporary Redirect](#307-temporary-redirect) (since HTTP/1.1)   
> [**308** Permanent Redirect](#308-permanent-redirect) (RFC 7538)  
> [**308** Resume Incomplete](#308-permanent-redirect) (Google)  


## 4xx Client Error  
> The 4xx class of status code is intended for cases in which the client seems to have erred. Except when responding to a HEAD request, the server should include an entity containing an explanation of the error situation, and whether it is a temporary or permanent condition. These status codes are applicable to any request method. User agents should display any included entity to the user.  

> [**400** Bad Request](#400-bad-request)  
> [**401** Unauthorized](#402-unauthorized) (RFC 7235)  
> [**402** Payment Required](#402-payment-required)  
> [**403** Forbidden](#403-forbidden)  
> [**404** Not Found](#404-not-found)  
> [**405** Method Not Allowed](#405-method-not-allowed)  
> [**406** Not Acceptable](#406-not-acceptable)  
> [**407** Proxy Authentication Required](#407-proxy-authentication-required) (RFC 7235)  
> [**408** Request Timeout](#408-request-timeout)  
> [**409** Conflict](#409-conflict)  
> [**410** Gone](#410-gone)  
> [**411** Length Required](#411-length-required)  
> [**412** Precondition Failed](#412-precondition-failed) (RFC 7232)  
> [**413** Payload Too Large](#413-payload-too-large) (RFC 7231)  
> [**414** Request-URI Too Long](#414-request-uri-too-long)  
> [**415** Unsupported Media Type](#415-unsupported-media-type)  
> [**416** Requested Range Not Satisfiable](#416-requested-range-no-satisfiable) (RFC 7233)    
> [**417** Expectation Failed](#417-expectation-failed)    
> [**418** I'm a teapot](#418-im-a-teapot)  
> [**419** Authentication Timeout](#419-authentication-timeout) (not in RFC 2616)  
> [**420** Method Failure](#420-method-failure) (Spring Framework)  
> [**420** Enhance Your Calm](#420-enhance-your-calm) (Twitter)  
> [**421** Misdirected Request](#421-misdirected-request) (HTTP/2)  
> [**422** Unprocessable Entity](#422-unprocessable-entity) (WebDAV; RFC 4918)  
> [**423** Locked](#423-locked) (WebDAV; RFC 4918)  
> [**424** Failed Dependancy](#424-failed-dependancy) (WebDAV; RFC 4918)  
> [**426** Upgrade Required](#426-upgrade-required)  
> [**428** Precondition Required](#428-precondition-required) (RFC 6585)  
> [**429** Too Many Requests](#429-too-many-requests) (RFC 6585)  
> [**431** Request Header Fields Too Large](#431-request-header-fields-too-large) (RFC 6585)  
> [**440** Login Timeout](#440-login-timeout) (Microsoft)  
> [**444** No Response](#444-no-response) (Nginx)  
> [**449** Retry With](#449-retry-with) (Microsoft)  
> [**451** Unavailable For Legal Reasons](#451-unavailable-for-legal-reasons) (Internet draft)  
> [**451** Redirect](#451-redirect) (Microsoft)  
> [**494** Request Header Too Large](#494-request-header-too-large) (Nginx)  
> [**495** Cert Error](#495-cert-error) (Nginx)  
> [**496** No Cert](#496-no-cert) (Nginx)  
> [**497** HTTP to HTTPS](#497-http-to-https) (Nginx)  
> [**498** Token expired/invalid](#498-token-expired-invalid) (Esri)  
> [**499** Client Closed Request](#499-client-closed-request) (Nginx)  
> [**499** Token Required](#499-token-required) (Esri)  



## 5xx Server Error  
> The server failed to fulfill an apparently valid request.  
> Response status codes beginning with the digit "5" indicate cases in which the server is aware that it has encountered an error or is otherwise incapable of performing the request. Except when responding to a HEAD request, the server should include an entity containing an explanation of the error situation, and indicate whether it is a temporary or permanent condition. Likewise, user agents should display any included entity to the user. These response codes are applicable to any request method.  

> [**500** Internal Server Error](#500-internal-server-error)  
> [**501** Not Implemented](#501-not-implemented)  
> [**502** Bad Gateway](#502-bad-gateway)  
> [**503** Service Unavailable](#503-service-unavailable)  
> [**504** Gateway Timeout](#504-gateway-timeout)  
> [**505** HTTP Version Not Supported](#505-http-version-not-supported)  
> [**506** Variant Also Negotiates](#506-variant-also-negotiates) (RFC 2295)    
> [**507** Insufficient Storage](#507-insufficient-storage) (WebDAV; RFC 4918)  
> [**508** Loop Detected](#508-loop-detected) (WebDAV; RFC 5842)  
> [**509** Bandwidth Limit Exceeded](#509-bandwidth-limit-exceeded) (Apache bw/limited extension)  
> [**510** Not Exteded](#510-not-extended) (RFC 2774)  
> [**511** Network Authentication Required](#511-network-authentication-required) (RFC 6585)  
> [**520** Unknown Error](#520-unknown-error)  
> [**522** Origin Connection Time-out](#522-origin-connection-time-out)  
> [**598** Network read timeout error](#598-network-read-timeout-error) (unknown)    
> [**599** Network connect timeout error](#599-network-connect-timeout-error) (unknown)    







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

#### 203 Non-Authoritative Information  
> (since HTTP/1.1)
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

#### 226 IM Used  
> (RFC 3229)
> The server has fulfilled a request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.  


#### 300 Multiple Choices    
> Indicates multiple options for the resource that the client may follow. It, for instance, could be used to present different format options for video, list files with different extensions, or word sense disambiguation.  

#### 301 Moved Permanently     
> This and all future requests should be directed to the given URI.  

#### 302 Found       
> This is an example of industry practice contradicting the standard. The HTTP/1.0 specification (RFC 1945) required the client to perform a temporary redirect (the original describing phrase was "Moved Temporarily"),[6] but popular browsers implemented 302 with the functionality of a 303 See Other. Therefore, HTTP/1.1 added status codes 303 and 307 to distinguish between the two behaviours.[7] However, some Web applications and frameworks use the 302 status code as if it were the 303.  

#### 303 See Other  
> (since HTTP/1.1)  
> The response to the request can be found under another URI using a GET method. When received in response to a POST (or PUT/DELETE), it should be assumed that the server has received the data and the redirect should be issued with a separate GET message.    

#### 304 Not Modified  
> (RFC 7232)  
> Indicates that the resource has not been modified since the version specified by the request headers If-Modified-Since or If-None-Match. This means that there is no need to retransmit the resource, since the client still has a previously-downloaded copy.  

#### 305 Use Proxy  
> (since HTTP/1.1)  
> The requested resource is only available through a proxy, whose address is provided in the response. Many HTTP clients (such as Mozilla and Internet Explorer) do not correctly handle responses with this status code, primarily for security reasons.  

#### 306 Switch Proxy     
> No longer used. Originally meant "Subsequent requests should use the specified proxy."    

#### 307 Temporary Redirect  
> (since HTTP/1.1)  
> In this case, the request should be repeated with another URI; however, future requests should still use the original URI. In contrast to how 302 was historically implemented, the request method is not allowed to be changed when reissuing the original request. For instance, a POST request should be repeated using another POST request.      
#### 308 Permanent Redirect  
> (RFC 7538)  
> The request, and all future requests should be repeated using another URI. 307 and 308 (as proposed) parallel the behaviours of 302 and 301, but do not allow the HTTP method to change. So, for example, submitting a form to a permanently redirected resource may continue smoothly.  

#### 308 Resume Incomplete  
> (Google)  
> This code is used in the Resumable HTTP Requests Proposal to resume aborted PUT or POST requests.  


#### 400 Title  
> text here.  

  
#### 500 Title  
> text here.  


