### Web Services 

1. [What is a web service?](#definition)
1. [Basic concept behind web services]()
1. [Why use it?](#why)
1. [Client Server model](#client-server)
1. [Types of web services - SOAP/REST](#types)
1. [Components of Web Services - WSDL, UDDI](#components)
1. [SOAP Web Services](#soap)
1. [REST Web Services](#rest)

<hr/>

#### <a id="definition">WebService -</a> 
* enables communucation between applications on the web.
* provides a standard protocol/format for communication.
* service available over the web.

#### <a id="why">Why Use WebServices -
* platform independent communication.
* allows two different applications to talk to each other and exchange information.
  
#### <a id="client-server">Client Server Model</a>
* Client sends request to the Server (service provider)
* Medium HTTP / Internet
* Format XML/JSON

#### <a id="types">Types of Web Services</a>
* SOAP - Simple Object Access Protocol
  - Medium HTTP (POST)
  - Format XML
  - Example
  ```xml
  ```
* REST - Representational State Transfer
  - Medium HTTP (POST,GET,PUT,DELETE,...)
  - Format XML/JSON/TEXT
  
#### <a id="components">Components of Web Services</a>
* WSDL - Web Services Description Language - An XML based interface that describes the functionalities of Web Services.
* UDDI - Universal Description, Discovery and Integration. - An XML based standard for publishing and finding web services.

#### <a id="soap">SOAP Web Services</a>
* Complies to the SOAP Web Services Specifiactions.
  - W3C (World Wide Web Consortium https://www.w3.org) - defines and dictates the standards.
* Specifications.
  - Basic
    * SOAP (Simple Object Access Protocol)
    * WSDL
    * UDDI
  - Extended
    - WS-Security
    - WS-Policy
    - ...
* Format
```soap
<?xml verstion="1.0"?>
<soap:Envelope 
      xmlns soap="http://www.w3.org/2001/12/soap-envelope"
      soap:encodingStyle="www.w3.org/2001/12/soap-encoding">
  <soap:body pb="http://www.example.com/employees">
    <pb:GetEmployee>
      <pb:EmpId>123</pb:EmpId>
    </pb:GetEmployee>
  </soap:body>
</soap:Envelope>
```
* Defined Structure
  - SOAP Message
    * Envelope
      * Header - Information about the message itself.
        - Authentication
        - Complex Types
        - Routing
      * Body - Actual data of the request.

#### <a id="rest">REST Web Services</a>

* REST - Representational State Transfer (architectural style) - Allows communication between 2 applications using REST architecture.
* Principles
  - Uniform interface
    - Resource - anything can be a resource
    - URI - resource can be accessed by uri
    - HTTP -make use of HTTP methods
      * GET - Read
      * POST - Add
      * PUT - Update
      * DELETE - Delete
    - Manipulation using Representations
      * application/xml
      * application/json
      * text/html
    - Descriptive Messages (how content should be handled)
      * caching
      * authentication
      * etc
  - Stateless
    - Communications are stateless (server does not maintain any state of the system - each request must contain all of the data needed for the request) 
  - Cacheable
    * Caching occurs at the client side
      * Cache-Control header to indicate whether to cache or not
  - Layered
    * Multiple layers can exist between client and server
      * Proxies
      * Gateways
      * etc
  - Code on Demand
* Format - Using GET
```rest
http://example.com/employees/123
```


[Back](../../tree/master)

