### Java Design Patterns

* Creational
  1. Singleton
  1. Factory
      1. Interface
      1. Classes implement Interface
      1. Class (factory) that returns an object 
  1. Abstract Factory
  1. Builder
      1. Similar to Factory Builder Class is used to Construct the object without having to know all of the parameters.
      ```java
      class PhoneBuilder
      {
          private String os = "IOS";
          int battery = 3100;
          
          public PhoneBuilder setOs(String os) {
              this.os = os;
              return this;
          }
          
          public PhoneBuilder setBattery(int battery) {
              this.battery = battery;
              return this;
          }
          
          public Phone getPhone() {
              return new Phone(os,battery);
          }
      }
      class Phone
      {
          private String os;
          private int battery;
          
          public Phone(String os, int battery) {
              this.os = os;
              this.battery = battery;
          }
          
          @Override
          public String toString() {
              return "Phone [os=" + os + ", battery=" + battery;
          }
      }
      class Shop
      {
          public static void main(String[] args) {
              Phone phone = new PhoneBuilder.setOs("Android").getPhone();
          }
      }
      ```
  1. Prototype
* Structural
  1. Adapter
  1. Composite
  1. Proxy
  1. Fly Weight
  1. Facade
  1. Bridge
  1. Decorator
* Behavioural
  1. Template Method
  1. Mediator
  1. Chain of Responsibility
  1. Observer
  1. Strategy
  1. Command
  1. State
  1. Visitor
  1. Iterator
  1. Interpreter
  1. Memento

1. [Singleton Design Pattern](singleton/README.md)
1. [Factory Design Pattern](https://howtodoinjava.com/design-patterns/creational/implementing-factory-design-pattern-in-java/)
1. Decorator Design Pattern
1. Composite Design Pattern
1. Adapter Design Pattern
1. Prototype Design Pattern
1. Facade Design Pattern
1. Proxy Design Pattern
1. Iterator Design Pattern

[Back](../../../tree/java/)

