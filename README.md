# Simple Microservice Project

This is simple microservice project. Consist of 5 service:

* Config Service
* Discovery Service
* Student Service 
* School Service
* Gateway

## Table of Contents

1. [Installation](#installation)
2. [Getting Started](#getting-started)
3. [Built With](#built-with)

## Installation

```
git clone https://github.com/nurananacafova/Simple-Microservice-Project.git
```

## Getting Started

* Run the project. Open the Postman

Example JSON format for create new Student:
```
{
    "firstName": "firstname_of_student", 
    "lastName": "lastname_of_student",
    "email": "student_email@example.com",
    "schoolId": school_id
}
```
Example JSON format for create new School:
```
{
    "name": "school_name",
    "email": "school_email@example.com"
}
```
#### WIth Api Gateway
* Add new student:

  Post request: http://localhost:8222/api/v1/students

* Add new school:

  Post request: http://localhost:8222/api/v1/schools

* Get all students:

  Get request: http://localhost:8222/api/v1/students

* Get all schools:

  Get request: http://localhost:8222/api/v1/schools

* Get schools with students:

  Get request: http://localhost:8222/api/v1/schools/with-students/{school-id}


### Without Api Gateway:

* Add new student:

  Post request: http://localhost:8090/api/v1/students

* Add new school:

  Post request: http://localhost:8070/api/v1/schools

* Get all schools:

  Get request: http://localhost:8070/api/v1/schools

* Get all students:

  Get request: http://localhost:8090/api/v1/students

## Built With

- Spring Boot
- Maven
- PostgreSQL
- Zipkin

#### Gateway:  http://localhost:8222/
#### Zipkin: http://localhost:9411/