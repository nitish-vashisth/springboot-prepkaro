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

# SpringBoot Security

- Spring Security
- 5 spring security concept
- Authentication	who is the user ?
- Authorization	Are they allowed to do certain things
- Principal	currently logged in user
- Granted Authority	way of providing Authorization.
- Roles	Group of authority


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


Referernces

| Link 													        	  | Topics   |
|-------------------------------------------------------------------------------------------------------------------------|----------|
|[Spring Boot Quick Start](https://www.youtube.com/watch?v=msXL2oDexqw&list=PLqq-6Pq4lTTbx8p2oCgcAQGQyqN8XeA1x)           |          |
| [Spring Security ]([url](https://www.youtube.com/watch?v=sm-8qfMWEV8&list=PLqq-6Pq4lTTYTEooakHchTGglSvkZAjnE)  	  |          |
| [Spring Boot Microservices Level ](https://www.youtube.com/watch?v=y8IQb4ofjDo&list=PLqq-6Pq4lTTZSKAFG6aCDVDP86Qx4lNas) | Communication and discovery |
|[Spring Boot Microservices Level 2](https://www.youtube.com/watch?v=o8RO38KbWvA&list=PLqq-6Pq4lTTbXZY_elyGv7IkKrfkSrX5e) |          |







