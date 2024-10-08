# Must know concepts before starting SpringBoot
- Framework
- Spring
- Inversion of Control (IOC)
- Spring Beans
- Dependency Injection
- Bean Scope
- Spring MVC
- Spring Webflux
- Aspect Oriented Programming (AOP)
- Spring AOP 

 Full Article : [Must know concepts before starting SpringBoot](https://prepkaro.com/must-know-springboot-concepts/)

 # Introduction

 

 # Restful Webservices

 Webservice -> Service that are exposed to internet for programmatic access

 Restful Web Services
 Soap Web Services

 ## Web Services Characteristic
HTTP request , HTTP Resonse (Http Exchange)
XML / jSON - Data format

### Protocol
Message Format (for ex Soap Protocol)
Rest -> There is not protocol

### Method
There is no rule. Though there is guideline

### Service Definition
Soap -> WSDL . And made availale to all client
Rest -> little to No Standard

SOAP web service specification

Rest - This is just an Idea. There are no rule

Rest -> Representational State Transfer

Rest + Web Service = Restful webservice 

Not Restful ---- Not Fully Restfull ---- Completely Restful

### Rest and HTTP

HTTP
HTML
Resource Location - API Address (Practice is to use resources based) should not be action based. Its just a lookup for something

HTTP Method
- Get
- Post
- Put
- Delete

A good Resfull api make a good choise of these menthods

Metadata
--> HTTP Status Code . Why send status code ?
--> Headers - Content type
--> Content negotiation

V-3









# Communication and Discovery
- Service Discovery
- Netflix Eureka

[Spring Boot Microservices Level - Communication and Discovery](https://www.youtube.com/watch?v=y8IQb4ofjDo&list=PLqq-6Pq4lTTZSKAFG6aCDVDP86Qx4lNas)

#  Fault Tolerance and Resilience
- Fault Tolerance
- Resilience
- Timeout Pattern
- Retry Pattern
- Fail Fast
- Circuit Breaker Pattern
- Bulkhead Pattern
- Rate Limiter
- resilience4j

 [Spring Boot Microservices Level 2 - Fault Tolerance and Resilience](https://www.youtube.com/watch?v=o8RO38KbWvA&list=PLqq-6Pq4lTTbXZY_elyGv7IkKrfkSrX5e)

# Microservice configuration





# springboot-champion

- Spring Version Currenlty Using
- SpringBoot Version Currenty Using
- Lates version for both

## What is Spring Boot ?

Spring Boot makes it easy to create stand-alone, production-grade Spring based Applications that you can "just run”.

## What is Spring?
•	Application Framework
•	Programming and configuration model
•	Infrastructure support

## Problem with Spring?
•	Huge Framework
•	Multiple setup steps
•	Multiple configuration steps
•	Multiple build and deploy step

#### Can we abstract these steps ?  
Yes, SpringBoot do that

#### Spring Boot features
•	Opinionated
•	Convention over configuration
•	Stand alone.
•	Production ready

## Build and dependency management.
	
## Maven 

## Creating a project
1.	Using Simple Maven Project and adding spring boot dependency


•	Spring-boot-starter-parent
•	spring-boot-starter-web
If we want to change the version of any dependency that we want to pull from the starter parent, we can add the dependency in the dependency tag and directly configure its property

<properties>
    <junit.version>4.11</junit.version>
</properties>


## Dependency vs Dependency Management


## @SpringBootApplication
https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/using-boot-using-springbootapplication-annotation.html
•	@EnableAutoConfiguration
•	@ComponentScan
•	@Configuration

## SpringApplication.run main method
https://stackoverflow.com/questions/24271705/springapplication-run-main-method


## Starting SpringBoot Application
•	Setup default configuration
•	Start Spring application context
•	Perform classpath scan
•	Starts Tomcat Server

## Common Annotation

Spring Common Annotation

@SpringBootApplication	@Getter	@RestController	
@EnableAutoConfiguration	@PostConstruct	@CrossOrigin	
@ComponentScan	@PreDestroy	@GetMapping	
@Configuration	@JsonInclude	@PostMapping	
@Component	@JsonIgnoreProperties	@Produces	
@EnableCaching	@JsonProperty	@Validated	
@Autowired	@Data	@PathVariable	
@Primary	@EnableRetry	@RequestBody	
@Service	@EnableListener	@ApiOperation	
@Qualifier	@EnableWebMVC	@ApiIgnore	
@Value	@ControllerAdvice	@Controller	
@Bean	@ExceptionHandler	@Repository


# Dependency Injection and Beans

### Constructor vs Field vs Setter Injection


# Spring Boot Data Access
    - Spring JPA
    - Spring JDBC
    - QueryMethod

# RESTful APIs with SpringBoot

# Spring Boot Profiles
    - different properties based on profiles (like QA, Production)


<!------------------------------------------------- Spring Security Concepts Starts ----------------------------------->


# SpringBoot Security

## Resources
- [What is Spring Security really all about? Java Brains Brain Bytes](https://www.youtube.com/watch?v=sm-8qfMWEV8&list=PLqq-6Pq4lTTYTEooakHchTGglSvkZAjnE)
- [Spring Security With JWT for REST API](https://www.toptal.com/spring/spring-security-tutorial)
- [Spring Security Architecture](https://spring.io/guides/topicals/spring-security-architecture)
- [Spring Security Interview Questions](https://www.interviewbit.com/spring-security-interview-questions/)
- [Top 22 Spring Security Interview Questions for Java Programmers](https://www.educative.io/blog/spring-java-interview-questions-practice#jdbc)
- [Top 12 Tips For API Security - Byte Byte Go](https://www.youtube.com/watch?v=6WZ6S-qmtqY)
  
## Spring Security

### 5 spring security concept

- Authentication
     ##### who is the user ?
	- Knowledege Based 
 	- Posession Based
  	- Multifactor Authentication (ex - 2 Factor)
  	  
- Authorization
     #### Are they allowed to do certain things
  
- Principal
     #### Currently logged in user.
  
- Granted Authority
     #### Way of providing Authorization
     #### Fine grained
  
- Roles
     #### Group of authority
     #### Coarsed grained

### Adding Spring Security to new Spring Boot project

   ##### Maven Dependency
   [Spring Boot with Maven](https://docs.spring.io/spring-security/reference/getting-spring-security.html#getting-maven-boot)

   
	  <dependency>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-security</artifactId>
	  </dependency>

   ##### Default Behaviour 
   - Add mandatory Authentication for URL
   - Add login form
   - Handle login Error
   - Create a user and set a default password
 
   ## configure Spring Security Authentication

   #### WebSecurityConfigurererAdapter
   	configure(AuthernticationManagerBuilder auth) -> Method
   #### AuthenticationManagerBuilder  -> for Authentication 
   #### Authentication manager
   	Authernticate() -> Method
  #### PasswordEncoder Bean
  #### HttpSeurity  --> For autherization
  	configure()

  ### Filters

  ### Other Concepts
  - JDBC
  - JPA - Java Peristenet API
  - [Spring Data](https://spring.io/guides/topicals/spring-security-architecture)
  - LDAP
  - JWT
  - OAuth

## Top 12 Tips For API Security
   #### 1. Use HTTPS
   #### 2. OAuth2
   #### 3. WebAuthn
   #### 4. Use Leveled API key and rotate periodically
   #### 5. Implement Authorization - Principle of least privilege
   #### 6. Rate limiting
   #### 7. Implement API versioning
   #### 8. Allow listing - Deny All approach, Allow List Approach
   #### 9. Check OWASP API security risk
   #### 10. API Gateway
   #### 11. Error handling - Do not explose sensitive info and anything in error message. Never return full stack trace etc.
   #### 12. Robust input validation - Client side vs server side

  - [Top 12 Tips For API Security - Byte Byte Go](https://www.youtube.com/watch?v=6WZ6S-qmtqY)
   
   


<!------------------------------------------------- Spring Security Concepts Ends ----------------------------------->


# Spring Boot Logging
 
# Spring Boot Exception Handling

# Spring Boot Caching

# Spring Boot Interceptor

# Spring Boot Scheduling

# SpringBoot Testing
    - Mockito

# Microservices with SpringBoot

## Introduction to Microservices
   - Introduction to Microservices

- Service Discovery using Eureka
    - Microservice Registering

- Tracing the request in multiple Microservices
    - Sleuth and Zipkin
    - Sleuth links the trace id with your request
    - Zipkin help to visualize using the trace id
 
# Spring Cloud Config Servers:
    - its Configuration managmenet

# Communition between different microservies 
    - SYNC
    - ASYNC (messaging queue)

# API Gateway

# Circuit Breaker

# CQRS (Command Query Responsibility Segregation)

# Deployment and Containerization
 - creating executable JARs and WARs


## What is a Servlet ?


	

    

14.

Other Questions


1.	What is ClassPath ?
2.	Artifact vs group id
3.	Jar vs war

Resource
1.	Java Brains


Spring Boot 
https://examples.javacodegeeks.com/spring-boot-interview-questions-and-answers/
https://www.interviewbit.com/spring-boot-interview-questions/

1.	Spring Framework vs Spring Boot

Dependecy Injection
Bean
ApplicatonContext
Classpath
Consutructer or Setter Injection

1. DI
2. Actuator 
3. Profiling: was able to explain the use of profiling and how to create / deploy 
4. Starter dependencies
5. Bean Scopes
Week Topic
Logging
application.yml vs application.properties for Spring Boot
https://stackoverflow.com/questions/47462950/application-yml-vs-application-properties-for-spring-boot

Interview Questions
Interview Bit ->  https://www.interviewbit.com/spring-boot-interview-questions/

ToDo:
1. Creating a custom springboot starter
2. Fault tolerance and resileince using Resileience4j


Referernces

| Link 													        	  | Topics   |
|-------------------------------------------------------------------------------------------------------------------------|----------|
|[Spring Boot Quick Start](https://www.youtube.com/watch?v=msXL2oDexqw&list=PLqq-6Pq4lTTbx8p2oCgcAQGQyqN8XeA1x)           |          |
| [Spring Security ](https://www.youtube.com/watch?v=sm-8qfMWEV8&list=PLqq-6Pq4lTTYTEooakHchTGglSvkZAjnE)  	          |          |
| [Spring Boot Microservices Level ](https://www.youtube.com/watch?v=y8IQb4ofjDo&list=PLqq-6Pq4lTTZSKAFG6aCDVDP86Qx4lNas) | Communication and discovery |
|[Spring Boot Microservices Level 2](https://www.youtube.com/watch?v=o8RO38KbWvA&list=PLqq-6Pq4lTTbXZY_elyGv7IkKrfkSrX5e) |          |




PrepKaro

[Must know concepts before starting SpringBoot](https://prepkaro.com/must-know-springboot-concepts/)


# Interview Questions

1. What is Spring boot ?
2. Features of SpringBoot 
3. Spring vs SpringBoot 
4. How SpringBoot works ?
5. @SpringBootApplication , @ComponentScan
6. What does the @SpringBootApplication annotation do internally?
7. @SpringBootApplication = { @Configuration, @EnableAutoConfiguration, @ComponentScan }
8. How does a spring boot application get started?
9. Spring Initializer
10. Starter dependencies?  [Top 7 Spring Boot Starters You Should Know in 2024 - Java Brains](https://www.youtube.com/watch?v=6sgjRygYVJk)
11. @RestController and @Controller
	[Answer1-StackOverflow](https://stackoverflow.com/questions/25242321/difference-between-spring-controller-and-restcontroller-annotation)
	[Answer1-StackOverflow](https://stackoverflow.com/questions/28646332/how-does-the-spring-responsebody-annotation-work)
12. IOC container
13. Describe the flow of HTTPS requests through the Spring Boot application ?
14. RequestMapping  vs GetMapping
15. Profiles in spring boot
16. Actuator
17. How to enable Actuator in Spring boot application ?
18. What are the actuator-provided endpoints used for monitoring the Spring boot application? (Health, Info, Beans, Mappings, Configprops, Httptrace, Heapdump, Threaddump, Shutdown)
19. How to enable debugging log in the spring boot application ?
20. Where do we define properties in the Spring Boot application ?
21. Dependency Injection
22. How to disable a specific auto-configuration class? @EnableAutoConfiguration(exclude={className})
23. Can we override or replace the Embedded tomcat server in Spring Boot?
24. Default port and how to change it ? 8080. It can be changed by adding sever.port properties in the application.property file.
25. Spring Boot dependency management
26. Spring Rest vs Jax-RS - [StackOverflow-Answer](https://stackoverflow.com/questions/42944777/difference-between-jax-rs-and-spring-rest)
27. JaxRs vs Jax-Ws - [StackOverflow-Answer](https://stackoverflow.com/questions/16539858/what-is-the-difference-between-jax-rs-and-jax-ws)
28. spring-boot-starters - custom spring boot starter
29. How to create a custom annotation
    

Source : 
[InterviewBit](https://www.interviewbit.com/spring-boot-interview-questions/)
[Backend Questions](https://roadmap.sh/questions/backend)
[RoadMap](https://roadmap.sh/spring-boot)




