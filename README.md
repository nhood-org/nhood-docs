# nhood Engine

## Problem

`nhood` (for neighborhood) is a data search engine based on a shortest geometrical distances between multidimensional metadata vectors. Engine maintains an universe of data with n-dimensional vectors of metadata as data description. On search the geometrically nearest objects are resolved and returned. 

## Use-cases

1. A resolution of nearest geographical locations around the user.

1. A resolution of content relevant to user preferences.

## Goal

The engine implementation if focused on:

- high performance
- resilience
- reactiveness
- cloud-nativeness

## Architecture

System architecture is based on containerized microservices principles. All of the components should be considered as a separate services that may consist of single or multiple instances of application container. Inter-service communication is based on a messaging/event bus. Service discovery, load balancing, container life cycle management is supported by container orchestration technology. 

![alt architecture](./images/nhood-architecture.png)

## Key Services

### Data layer services

- `Data URL Service`: 

    Simple CRUD data abstraction service for data url entities.
    
   Repository: https://github.com/nhood-org/nhood-data-url-svc 
   
   Application: https://nhood-data-url-svc.herokuapp.com/swagger-ui.html

   [![CircleCI](https://circleci.com/gh/nhood-org/nhood-data-url-svc.svg?style=shield)](https://circleci.com/gh/nhood-org/nhood-data-url-svc) [![Heroku](http://heroku-badge.herokuapp.com/?app=nhood-data-url-svc&style=flat&svg=1)](https://dashboard.heroku.com/apps/nhood-data-url-svc)

- `Data Matrix Service`: 

    Service maintaining a model of n-dimensional data grid, grouped into small and easy-to-compute data grid chunks, optimized for retrieval of data by vector elements.

### Engine services

- `Data Orchestrations Service`: 

    Service for orchestration of data registration and data resolution.

- `Data Finder`: 

    Engine service resolving nearest data.

### Frontal services

- `Api Gateway`: 

    Frontal gateway for web application

    Repository: https://github.com/nhood-org/nhoog-api-gateway

- `Admin Api Gateway`: 

    Frontal gateway exposing auxiliary UI consoles

- `Web Frontend`: 

    Container with web application

### Auxiliary services

- `Admin Service`:

    Spring Boot admin service
    
    Repository: https://github.com/nhood-org/nhood-admin

- `Discovery Service`:

    Eureka supporting Admin and Configuration services
    
    Repository: https://github.com/nhood-org/nhood-discovery-svc

- `Configuration Service`:

    Remote configuration provider
    
    Repository: https://github.com/nhood-org/nhood-config

Other Repositories:

- Parent BOM: https://github.com/nhood-org/nhood-parent-bom

    [![CircleCI](https://circleci.com/gh/nhood-org/nhood-parent-bom.svg?style=shield)](https://circleci.com/gh/nhood-org/nhood-parent-bom) 
    
- Parent Service BOM: https://github.com/nhood-org/nhood-parent-service-bom

    [![CircleCI](https://circleci.com/gh/nhood-org/nhood-parent-service-bom.svg?style=shield)](https://circleci.com/gh/nhood-org/nhood-parent-service-bom) 

- Maven repository: https://github.com/nhood-org/nhood-repository

## Technology

Core parts of implementation are based on:

- Spring Boot 2.x stack
- Spring Framework 5, Spring Cloud, Project React, RSocket
- Couchbase, R2DBC
- Docker, Docker Compose, Docker Swarm/Kubernetes
- JUnit5, Spock

## Road map

Road map may be found [here](./ROADMAP.md).
