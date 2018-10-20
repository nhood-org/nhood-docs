# nhood Road map

## Phase 1: 

Implementation of Location Service

- [x] NH001: Implement LocationEntry data model
- [x] NH002: Implement basic LocationEntry CRUD functionalities with REST controller
- [@] NH003: Setup CI/CD for Location Service

## Phase 2: 

Setup Location DB

- [ ] NH004: Setup Location DB
- [ ] NH005: Setup CI/CD for Location DB

## Phase 2: 

Message Bus

- [ ] NH006: Implement event handling for LocationEntry creation
- [ ] NH007: Setup message bus
- [ ] NH008: Integrate Location Service with message bus

## Phase 3:

Location Orchestration Service and location registration

- [ ] NH009: Implement location registration within Location Orchestration Service
- [ ] NH010: Setup CI/CD for Location Orchestration Service

## Phase 4:

Api Gateway

- [ ] NH011: Create Api Gateway service
- [ ] NH012: Expose location registration endpoint
- [ ] NH013: Expose location CRUD endpoints
- [ ] NH014: Setup CI/CD for Api Gateway service

## Phase 5

Neighborhood Finder

- NH015: Implement trivial resolution logic
- NH016: Setup CI/CD for Neighborhood Finder
- NH017: Integrate Location Orchestration Service with Neighborhood Finder

## Phase 6

Performance testing

- NH018: Configure jMeter for performance testing
- NH019: Implement test scenarios
- NH-20: Perform performance tests
