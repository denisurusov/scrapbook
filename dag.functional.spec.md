# AML Evidence Flow DAG

## Goals and constraints

### Goals

- Scale through supporting multiple AML evidence providing streams (decoupling)
- Transparency into evidence collection process

### Constraints (must have requirements)

#### Security

- Data provider authentication (signed by)
- Source tracing
- Tamper-proof

#### Functional

- Data and documents, directly or via DMC links
- API and browsing UI
- Data keyed off GFCID

## Moving parts (Actors)

### Providers (point of data collection)

- Vendors
- FinTech
- Internal onboarding and operations platforms

### Consumers (point of data usage)

- Data Validation (BSU checking)
- AML Review

Consumers should have a capability to reject data, in which case a formal set of data validation rules must be referenced

### Data flow

A mechanism that delivers data from the providers to the consumers, consisting of the following:

- an API to accept data
- a data store
- an API to consume data

"API" in this context refers to either push or pull delivery method

## Referenced DAGs

- eLake DAG
- Data Architecture DAG
