# springboot-champion


1.	What is Spring Boot ?
Spring Boot makes it easy to create stand-alone, production-grade Spring based Applications that you can "just run”.

2.	What is Spring?
•	Application Framework
•	Programming and configuration model
•	Infrastructure support

3.	Problem with Spring?
•	Huge Framework
•	Multiple setup steps
•	Multiple configuration steps
•	Multiple build and deploy step

Question : Can we abstract these steps ?  
Ans : Yes, SpringBoot do that

5.	Spring Boot features
•	Opinionated
•	Convention over configuration
•	Stand alone.
•	Production ready

6.	Build and dependency management.
1.	Maven 

7.	Creating a project
1.	Using Simple Maven Project and adding spring boot dependency


•	Spring-boot-starter-parent
•	spring-boot-starter-web
If we want to change the version of any dependency that we want to pull from the starter parent, we can add the dependency in the dependency tag and directly configure its property

<properties>
    <junit.version>4.11</junit.version>
</properties>


8.	Dependency vs Dependency Management


9.	@SpringBootApplication
https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/using-boot-using-springbootapplication-annotation.html
•	@EnableAutoConfiguration
•	@ComponentScan
•	@Configuration

10.	SpringApplication.run main method
https://stackoverflow.com/questions/24271705/springapplication-run-main-method


11.	Starting SpringBoot Application
•	Setup default configuration
•	Start Spring application context
•	Perform classpath scan
•	Starts Tomcat Server


12.	What is a Servlet ?


13.	Spring Common Annotation

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

    

14. Constructor vs Field vs Setter Injection



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






Spring Security
5 spring security concept
Authentication	who is the user ?
Authorization	Are they allowed to do certain things
Principal	currently logged in user
Granted Authority	way of providing Authorization.
Roles	Group of authority


