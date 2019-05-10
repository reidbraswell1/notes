### Spring Overview

* Client --> web.xml --> Request (send all requests to the dispatcher servlet)
* Front Controller - Dispatcher Servlet (checks xml configuration file)
```xml
<servlet>
<servlet-class>
   org.springframework.web.servlet.DispatcherServlet
</servlet-class>
</servlet>
```
* Annotation @Controller
