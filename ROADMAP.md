# nhood Road map

## Phase 1: 

Implementation of Data Url Service

- [ ] First project configuration
- [x] Implement DataUrl data model
- [x] Implement basic DataUrl CRUD functionalities with REST controller
- [x] Setup CI/CD for Data Url Service

## Phase 2:

Data Orchestration Service and data registration

- [ ] Implement data registration within Data Orchestration Service
- [ ] Setup CI/CD for Data Orchestration Service

## Phase 3: 

Message Bus

- [ ] Implement event consumption for DataUrl creation in Data Url Service
- [ ] Implement event publishing for DataUrl creation in Data Orchestration Service
- [ ] Setup message bus
- [ ] Integrate Data Url Service and Data Orchestration Service with message bus

## Phase 4:

Api Gateway

- [ ] Create Api Gateway service
- [ ] Expose data registration endpoint
- [ ] Expose data url CRUD endpoints
- [ ] Setup CI/CD for Api Gateway service

## Phase 5

Data Finder

- [ ] Implement trivial resolution logic without Data Matrix Service being used
- [ ] Setup CI/CD for Data Finder
- [ ] Integrate Data Orchestration Service with Data Finder

## Phase 6

Performance testing

- [ ] Configure jMeter for performance testing
- [ ] Implement test scenarios
- [ ] Perform performance tests

## Phase 7: 

Setup Data Url DB

- [ ] Setup Data Url DB
- [ ] Setup CI/CD for Data Url DB
