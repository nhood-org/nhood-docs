# nhood Engine

## Problem

`nhood` (for neighborhood) is an engine maintains a collection of location pointers all around the world and provides fast resolution of latest and closest neighbors to the given input pointer.

## Goal

The engine implementation if focused on:

- high performance
- resilience
- reactiveness

## Architecture

System architecture is based on containerized microservices principles. All of the components should be considered as a separate services that may consist of single or multiple instances of application container. Inter-service communication is based on an event bus. Service discovery, load balancing, container life cycle management is supported by Kubernetes. 

![alt architecture](./images/nhood-architecture.png)

## Services

### Data layer services

- `Location Service`: 

    Simple CRUD data abstraction service for location entities
    
    Repository: https://github.com/nhood-org/nhood-location-svc

- `User Service`: 

    Simple CRUD data abstraction service for user entities

### Engine services

- `User Orchestrations Service`: 

    Service for orchestration of user management

- `Location Orchestrations Service`: 

    Service for orchestration of location registration and location resolution

- `Neighborhood Finder`: 

    Engine service resolving nearest neighbor locations

### Frontal services

- `Api Gateway`: 

    Frontal gateway for web application

- `Admin Api Gateway`: 

    Frontal gateway exposing auxiliary UI consoles

    Repository: https://github.com/nhood-org/nhoog-api-gateway

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

- Jenkins: https://github.com/nhood-org/nhood-jenkins
- Parent BOM: https://github.com/nhood-org/nhood-parent-bom
- Parent Service BOM: https://github.com/nhood-org/nhood-parent-service-bom

## Technology

Core parts of implementation are based on:

- Spring Boot 2.x stack
- Spring Framework 5 cloud and reactive technologies
- Couchbase
- Docker, Kubernetes
- Jenkins, Nexus

## Road map

Road map may be found [here](./ROADMAP.md).
