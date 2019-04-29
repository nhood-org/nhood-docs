# nhood Road map

## Current goal

At the end of the road presented here a basic, simplified and even trivial implementation of core components is covered. Basic project configurations, documentation and what's the most important performance and unit testing are implemented. Such stage may be considered as a baseline for further sophisticated implementation of the engine. This baseline will help in proper asessment of improvements achieved during the course of project development.

## Phase 1: 

~~Implementation of Data Url Service~~

- [x] First project configuration
- [x] Implement DataUrl data model
- [x] Implement basic DataUrl CRUD functionalities with REST controller
- [x] Setup CI/CD for Data Url Service

## Phase 2:

~~Data Orchestration Service and data registration~~

- [x] Implement data registration within Data Orchestration Service
- [x] Setup CI/CD for Data Orchestration Service

## Phase 3: 

~~Message Bus~~

- [x] Implement event consumption for DataUrl creation in Data Url Service
- [x] Implement event publishing for DataUrl creation in Data Orchestration Service
- [x] Setup message bus
- [x] Integrate Data Url Service and Data Orchestration Service with message bus
- [x] Implement messaging testing tool

## Phase 4:

~~Api Gateway~~

- [x] Create Api Gateway service
- [x] Expose data registration endpoint
- [x] Expose data url CRUD endpoints
- [x] Setup CI/CD for Api Gateway service

## Phase 5

Data Finder

- [ ] Implement resolution engine logic with in memory data matrix
- [x] Implement performance testing for data finder library
- [x] Implement unit testing for data finder library
- [ ] Setup CI/CD for Data Finder
- [ ] Integrate Data Orchestration Service with Data Finder

## Phase 6

Performance testing

- [ ] Configure jMeter for e2e performance testing
- [ ] Implement test scenarios
- [ ] Perform performance tests

## Phase 7: 

Setup Data Url DB

- [ ] Setup Data Url DB
- [ ] Setup CI/CD for Data Url DB
