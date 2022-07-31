# private-parking-control-api

CRUD project for Private Parking Control.

## Technologies

- [Git](https://git-scm.com)
- [Java 11](https://www.oracle.com/br/java/technologies/javase/jdk11-archive-downloads.html)
- [Sprint Boot 2.7.2](https://spring.io/projects/spring-boot)
- [Maven](https://maven.apache.org/download.cgi) 
- [PostgreSQL](https://www.postgresql.org/download/)
- [IntelliJ IDEA](https://www.jetbrains.com/pt-br/idea/)
- [Eclipse](https://www.eclipse.org/downloads/) *Alternative IDE for IntelliJ IDEA*
- [Postman](https://www.postman.com/downloads/)
- [Insomnia](https://insomnia.rest/download) *Alternative for Postman*


## Clone the project

SSH:
```bash
git clone git@github.com:georgewcf/private-parking-control-api.git
```
ou HTTPS:
```bash
git clone https://github.com/georgewcf/private-parking-control-api.git
```


>In this application, you can to CREATE, READ, UPDATE and DELETE parking informations.
For this, run the application and choose your command in the Postman (GET, DELETE, PUT or DELETE).

Example: 

POST
```bash
- Select 'POST' type, click on 'Body', click on 'raw' and change 'Text' for 'JSON';
- Paste this URI label: http://localhost:8080/parking-spot;
- Copy this sample json informations and paste on postman. Click on 'Send';
  Your status response will be '201 Created'.
{
    "parkingSpotNumber": "E110",
    "licensePlateCar": "ABC3FG",
    "brandCar": "HYUNDAI",
    "modelCar": "HB20",
    "colorCar": "WHITE",
    "responsibleName": "Maria Ilda",
    "apartment": "110",
    "block": "E"
}{
    "parkingSpotNumber": "E110",
    "licensePlateCar": "ABC3FG",
    "brandCar": "HYUNDAI",
    "modelCar": "HB20",
    "colorCar": "WHITE",
    "responsibleName": "Maria Ilda",
    "apartment": "110",
    "block": "E"
}
```
GET
```bash
- Select 'GET' type
- Paste this URI label: http://localhost:8080/parking-spot and click on 'Send'.
  Your status response will be '200 OK'.
```

PUT
```bash
- Select 'PUT' type
- Paste this URI label: http://localhost:8080/parking-spot/{id} and click on 'Send'.
    *The value {id} you will be find using the 'GET' method. This value is an AUTO GENERATE. Copy and paste on URI.
  Your status response will be '200 OK'.

```

DELETE
```bash
- Select 'DELETE' type
- Paste this URI label: http://localhost:8080/parking-spot/{id} and click on 'Send'.
    *The value {id} you will be find using the 'GET' method. This value is an AUTO GENERATE. Copy and paste on URI.
  Your status response will be '200 OK'.
```
