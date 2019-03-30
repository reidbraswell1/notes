# Spring

[Spring Modules](https://docs.spring.io/spring-framework/docs/3.0.0.RC3/spring-framework-reference/html/ch01s02.html)

[Bean Scopes](https://docs.spring.io/spring/docs/3.0.0.M3/reference/html/ch04s04.html)

1. Is Spring Framework a lightweight or heavyweight solution ?  __lightweight__
1. Is AOP (Aspect Oriented Programming) part of the core container in Spring Framework ? __Spring IoC (Inversion of Control) container does not depend on AOP__
1. Is expression language part of the core container ? __Yes__
1. Is JMS (Java Message Service) part of the Data Access Layer in Spring ? __Yes__
1. Can Spring and Struts be integrated ? __Spring can be integrated with Struts 2__
1. How do you get the object of DAO (Data Access Object) in Spring Framework ? __dependency injection__
1. In which Spring version were Java 5 features introduced ? __3.0__
1. Which spring version introduced Spring Expression Language ? __3.0__
1. Which class would represent the spring IoC (Inversion of Control) container ? __Application Context__
1. How would you use the idref (pass the id of a bean to another bean) in spring framework ? __setter method and constructor argument__
1. How do you use the \<ref\> tag in spring ?  __bean id__
1. How would you define an inner bean in spring ? __\<property/\> or \<constructor-arg/\>__
1. Which spring property is replaced by c-namespace ? __\<constructor-arg/\>__
1. What is the scope of a bean by default ? __Singleton Scope__
1. What is the scope of a stateful (carry state - instance variables) bean ? __Prototype Scope__
1. Is a spring bean eagerly initialized in spring (default) ? __yes__
1. Is a spring bean autowired (default) ? __yes__
1. ApplicationContextAware does what ? __makes a bean aware to the container__
1. Scope of a stateless bean ? __Singleton__
1. In which scope can only a single bean created ? __singleton__
1. In which scope can any number of instances of a bean be created ? __prototype__
1. If a bean is limited only to HTTP request what is that called ? __request scope__
1. If a bean is limited only to HTTP session what is that called ? __session scope__
1. What is the scope for portlet context ? __global session scope__
1. In which version was thread scope introduced ? __3.0__
1. What is a gracefull way of shutting down the Spring IoC containger in non-web applications ? __registerShutdownHook()__
1. What would be a good way of controlling a bean lifescycle in spring ? __InitializingBean and DisposableBean also init() method__ 

