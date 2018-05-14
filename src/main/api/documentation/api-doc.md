** Overview **
---
Case Management service is an Enterprise level service that gives the ability to create and update cases/activities between various systems within the landscape. This service provides the flexibility of requesting for a case/activity creation/updation either using the canonical data model or native format of a consuming system.

** Getting Started **

RESTful API Modeling Language (RAML) makes it easy to manage the whole API lifecycle from design to sharing. It's concise - you only write what you need to define - and reusable. It is machine readable API design that is actually human friendly.
The below spec describes the Channel Payments Management REST API.

** Release Notes **

|Version|Release Date|Release Description|
|:-------:|:-----------:|:-------------------:|
|v1|5/12/2016|Initial version of the API implementation|
|||Support for *case* resource|


** API Specification **
---

**API Security**

The API is secured using Basic Authentication. Every request to the API *must* include the HTTP Authorization header with valid username & password. If the authentication is denied by the API, a 401 response will be sent back in response. The Authorization header is constructed as below:
1. The username and password are combined with a single colon.
2. The resulting string is encoded using the RFC2045-MIME variant of Base64, except not limited to 76 char/line.
3. The authorization method and a space i.e. "Basic " is then put before the encoded string.  

Example HTTP request header that contains the Authorization header

```
GET /payments HTTP/1.1
Host: www.esb-dev.hydrotasmania.com/case_management/v1/api
Authorization: Basic aHR0cHdhdGNoOmY=
```

** Support **
---

** Contact Us **
TBD

** FAQ **
TBD