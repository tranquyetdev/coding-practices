# Goals

Building a full example to solve a common business problem along with learning, and practicing new technologies in both DevOps and software Development such as:

- **Frontend**: Learning and practicing modern frontend frameworks, tools (NextJS, Remix, React native, CRA, etc)

- **Backend**: Learning and practicing microservices-based architecture, better understanding its pros and cons while developing a real project.
- **GraphQL**: Learning and building a [Hybrid approach](https://www.howtographql.com/basics/3-big-picture/). Interested in [federation architecture](https://www.apollographql.com/docs/federation/) for better support backend microservices
- **Caching**: Backend distributed caching and frontend graphql client caching
- **Message Queue**: A message queue for asynchronous communication between microservices
- **Logging**: End to end logging
- **Mornitoring**: Mornitoring the entire application with modern tools (using both cloud services or opensource libraries), including sending alerts, synthetic monitoring, etc.
- **Security**: Learning and Building applications with security in mind.
- **Monorepo**: Learning and practicing both software development, building the CI/CD pipeline, all in one with monorepo support.

# Architecture Overview

A draft architecture to represent components of the system, and what will be built. It could be changed during the learning process.

![High level architecture overview](solution.drawio.png 'High level architecture overview').

# Technology Stack

| Components          | Prefer                              | Alternative                 |
| ------------------- | ----------------------------------- | --------------------------- |
| frontend-web        | remix                               | nextjs                      |
| admin-web           | reactjs                             |                             |
| frontend-mobile     | react-native                        | flutter                     |
| GraphQL Gateway     | nestjs + apollo federation          | Apollo Managed Federation   |
| user-service        | nestjs microservice + apollo server | AWS AppSync                 |
| product-service     | nestjs microservice + apollo server | AWS AppSync                 |
| customer-service    | nestjs microservice + apollo server | AWS AppSync                 |
| order-service       | nestjs microservice + apollo server | AWS AppSync                 |
| recognition-service | --                                  |                             |
| message-queue       | redis (pub-sub)                     | RabbitMQ, Apache Kafka, SQS |
| distributed-cache   | redis (cluster mode)                | AWS Elasticache             |
| user-db             | TBD                                 |                             |
| product-db          | TBD                                 |                             |
| customer-db         | TBD                                 |                             |
| order-db            | TBD                                 |                             |
| logging             | TBD                                 |                             |
| monitoring          | TBD                                 |                             |
| security            | TBD                                 |                             |
| CI/CD               | Github Actions                      | CircleCI, SemaphoreCI       |
| IoC                 | Terraform                           |                             |
| monorepo            | NX                                  | turborepo                   |

# Implementation Detail

TBD

# Deployment

## Approach 1 - Deploy all components in a Kubernetes cluster

### 1.1 Deploy to EKS

TBD

### 1.2 Deploy to GKE

TBD

### 1.3 Deploy to AKS

TBD

## Approach 2 - Deploy AWS's services-based components

TBD
