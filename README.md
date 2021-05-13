# Cloudcluster
Deploying Spring-Boot in cloudclusters.io 

Deploying Spring-Boot in cloudclusters.io is same as deploying it in external tomcat in your device. cloudclusters offer cloudservices at low cost with one month ree trial without card details and have a wide range of service history. It'll be useful if You are looking for low costing services you can go for cloudcluster. 

Step 1: Extract .war file rom your spring boot app

i) Add/change packaging format to your project's pom.xml file:

	<groupId>com.gugan</groupId>
	<artifactId>Gugan</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<packaging>war</packaging>
	<name>Gugan</name>
	<description>Demo project for Spring Boot</description>
  
  
  ii)  Add the Tomcat dependency:

<dependencies>
<dependency>
   <groupId>org.springframework.boot</groupId>
   <artifactId>spring-boot-starter-tomcat</artifactId>
   <scope>provided</scope>
</dependency>
</dependencies>


iii) Initialize the Servlet context required by Tomcat by implementing the SpringBootServletInitializer interface:


@SpringBootApplication
public class GuganApplication extends SpringBootServletInitializer {
}


iv) execute the mvn clean package in cmd prompt 

C:\Users\path\Gugan> mvn clean package

Step 2:  Create a Java+Tomcat product by selecting the requirements 

Step 3:  Click on manage and go to file manager. Place your .war file inside tomcat/webapps and it'll extract the war file.

