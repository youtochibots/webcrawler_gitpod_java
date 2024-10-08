[![Ouvrir dans Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/youtochibots/webcrawler_gitpod_java)
# Web Crawler using Spring Boot and Completable Futures & EhCache

Ce projet eswebcrwler
## Prérequis

- Java 17
- Maven
- Un IDE comme IntelliJ IDEA ou Eclipse

## Installation

1. Clonez le dépôt:
   ```bash
   git clone https://github.com/maxds-lyon/Kata-Spring.git
   cd Kata-Spring
   ```

2. Construisez le projet avec Maven:
   ```bash
   mvn clean install
   ```

3. Lancez l'application Spring Boot:
   ```bash
   mvn spring-boot:run
   ```

# Web Crawler using Spring Boot and Completable Futures & EhCache

An example application using Spring boot and Completable Future & EhCache

## Technology stack
-   Spring Boot
-   Swagger
-   Spring Boot Test/JUnit/Mockito/RestAssured

## Build Instruction
- Maven
- JDK 8 or above

## Run

### Internet Without proxy
mvn spring-boot:run

### Internet With proxy

|   JVM Property     |Description           
|----------------|------------------------
|http.proxyHost  | proxy host name        
|https.proxyHost | https proxy host name  
|http.proxyPort  | proxy port number      
|https.proxyPort | https proxy port number
|http.proxyUser  | proxy user name        
|https.proxyUser | https proxy user name  
|http.proxyPassword  | proxy user password
|https.proxyPassword | https proxy user password


Pass all applicable jvm arguments
 
mvn -D[jvmProperty]=[value] spring-boot:run


### Testing

Endpoint:

http://localhost:8080/crawl?depth=5&breadth=10&url=https://example.com

|  Query Param name       |Description           |
|----------------|------------------------|
|url             | [Mandatory] url to crawl        |
|depth | Depth of the page links to be crawled, default is 2 max 10  |
|breadth  | Max number of page links to be considered to crawl, default is 10 and max 20      |

