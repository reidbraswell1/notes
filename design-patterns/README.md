### Java Design Patterns

* Creational
  1. Singleton
  1. Factory
      1. Interface
      1. Classes implement Interface
      1. Class (factory) that returns an object
      ```java
        interface OS
        {
            void spec();
        }
        class Android implements OS
        {
            void spec() {
                System.out.println("Good OS");
            }
        }
        class IOS implements OS
        {
            void spec() {
                System.out.println("Better OS");
            }
        }
        class OSFactory
        {
            public OS getInstance(String os) {
                if(os == "IOS") {
                    return new IOS();
                 }
                 else {
                    return new Android();
                 }
            }
        }
        class FactoryMain 
        {
            public static void main(String[] args) {
                OSFactory osf = new OSFactory();
                OS os = osf.getInstance("Android");
            }
        }
      ```
  1. Abstract Factory
  1. Builder
      1. Similar to Factory - Builder Class is used to Construct the object without having to know all of the constructor parameters and parameters can be added in any order by setter chaining.
      ```java
      class PhoneBuilder
      {
          private String os = "IOS";
          private int battery = 3100;
          private String color = "White";
          
          public PhoneBuilder setOs(String os) {
              this.os = os;
              return this;
          }
          
          public PhoneBuilder setBattery(int battery) {
              this.battery = battery;
              return this;
          }
          
          public PhoneBuilder setColor(String color) {
              this.color = color;
              return this;
          }
          
          public Phone getPhone() {
              return new Phone(os,battery,color);
          }
      }
      class Phone
      {
          private String os;
          private int battery;
          private String color;
          
          public Phone(String os, int battery, String color) {
              this.os = os;
              this.battery = battery;
              this.color = color;
          }
          
          @Override
          public String toString() {
              return "Phone [os=" + os + ", battery=" + battery + ", color=" + color + "]";
          }
      }
      class Shop
      {
          public static void main(String[] args) {
              Phone phone = new PhoneBuilder().setOs("Android").setColor("Blue").getPhone();
              System.out.println(phone);
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

