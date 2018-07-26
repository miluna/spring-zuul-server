# Spring Zuul Server - Proxy Gateway
Base project using Netflix Zuul with Netflix Eureka Server. Zuul works as a Proxy Gateway to other registered services with Eureka.

Make sure you set your Eureka address in the application.yml


```yml

#Server Port
server:
  port: 8765

#EUREKA
eureka:
  client:
    registerWithEureka: true
    fetchRegistry: true
    serviceUrl:
      defaultZone: http://localhost:8761/eureka/
  instance:
    preferIpAddress: true
```
