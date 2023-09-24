# Task 1

### Requirements

- Java
- Maven
- Spring Boot (Framework)
- MongoDB

#### Dependencies

- spring-boot-starter-web
- spring-boot-starter-data-mongodb
- spring-boot-maven-plugin

## Building steps

1. Run `mvn clean install`
   This will build and install the artifacts in to the local repository.
   Required jar file will be created inside `/target` folder.

2. Run the application by clicking `Run` option or pressing `F9`
   SpringBoot application server will load and start on port `8080` of the `localhost`.

## Rest API Endpoints and Resources

Rest API Endpoint is mapped to `http://127.0.0.1:8080/servers/`

- PUT a server `http://127.0.0.1:8080/servers/createServer`
  Accept "server" object in body in json format.

- GET servers `http://127.0.0.1:8080/servers/getServer`
  Returns a list of "server" objects.

- GET server by ID `http://127.0.0.1:8080/servers/getServer?id=<ID>`
  Returns a "server" object matching with ID.

- GET servers by Name `http://127.0.0.1:8080/servers/getServer?name=<Nmae>`
  Returns a list of "server" objects matching with Name.

- DELETE server `http://127.0.0.1:8080/servers/deleteServer?id=<ID>`
  Deletes a "server" object matching with ID.

### Screenshots of Output

![CreateServer](/output/1.png)

![GetServer](/output/2.png)

![GetServById](/output/3.png)

![GetServByIdAgain](/output/4.png)

![DelById](/output/5.png)
