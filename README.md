# Library Management System
Gold Coast IT Library Management System

This is the main repository for the Library Management System. There are several Git submodules within this repository. To clone this repository with all submodules use the git --recursive flag.

git clone --recursive https://github.com/tbreitenfeldt/library-management-system.git

Each submodule is a microservice that is apart of this project.

## Description

This project provides the functionality needed to run a library, covering the three basic user types: borrower, librarian, and admin. This allows average users to checkout and checkin books, librarians to manage the library branch they work for, and admins to control everything through CRUD (Create, Read, Update, and Delete) operations on all resources.

All of the backedn microservices, borrower-microservice, librarian-microservice, and admin-microservice, are written in spring boot using spring data JPA, where the front end service, ng-lms, is written in angular. Swagger documentation is included in the microservices-single-swagger submodule. Security is implemented using Spring Secuirty through the orchestrator-service, which acts as the primary gateway for the backend services. The Orchestrator leverages Eureka in the eureka-microservice submodule to handle service discovery and load balancing.

#### Included Submodules

- borrower-microservice
- librarian-microservice
- administrator-microservice
- orchestrator-microservice
- eureka-microservice
- microservices-single-swagger
