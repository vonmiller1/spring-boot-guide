# Spring Boot Guide

A structured, self-paced learning path and reference collection for backend developers moving from Java fundamentals to production-minded Spring Boot applications.

## Overview

This repository is a **documentation-only** guide: there is no application code, build file, or runtime to install. It organizes a multi-phase roadmap, curated external resources, project ideas, interview preparation links, and downloadable cheatsheets so you can study Spring Boot without hunting across scattered bookmarks.

The path emphasizes learning by building—each phase suggests practice work, and companion documents list projects by difficulty and quality standards aligned with real backend engineering.

## Features

- Phased roadmap from Java foundations through advanced topics (messaging, microservices, observability).
- Progress checklist to track topics as you practice them.
- [Project ideas](Project%20Roadmap%20and%20Projects.md) grouped by difficulty with extension challenges.
- [Learning resources](Recommended%20Learning%20Resources.md) with links to official documentation and optional courses.
- [Interview preparation](Interview%20Preparation.md) curated question collections and a practice workflow.
- [Cheatsheets](Cheatsheets.md) for Git, SQL, Docker, Maven, Spring annotations, and related references.
- Visual roadmap graphic (embedded below and in [Downloadable Springboot roadmap.md](Downloadable%20Springboot%20roadmap.md)).

## Tech stack

| Area | Details |
| --- | --- |
| Content format | Markdown (`.md`) |
| Version control | Git |
| Hosting | GitHub (static documentation) |

There is no Java, Spring Boot, Maven, or Gradle project in this repository. Apply the roadmap in your own practice repositories.

## Prerequisites

- A web browser to read the guides on GitHub or locally.
- [Git](https://git-scm.com/downloads) if you want to clone or contribute.
- For **following** the roadmap (outside this repo): a JDK supported by your chosen Spring Boot version, Maven or Gradle, and optionally Docker—see the phase descriptions below.

> **Version note:** Java and Spring release support changes over time. Choose a supported Java version for the Spring Boot release you use, and check the [Spring Boot reference documentation](https://docs.spring.io/spring-boot/reference/) before starting a new project.

## Getting started

```bash
git clone https://github.com/vonmiller1/spring-boot-guide.git
cd spring-boot-guide
```

Open `README.md` in your editor or view the repository on GitHub. No environment variables or secrets are required to use this guide.

## Running locally

This repository does not run as a service. After cloning, browse the Markdown files directly or use any Markdown preview in your IDE. External PDF and image assets linked from [Cheatsheets.md](Cheatsheets.md) are hosted on GitHub user attachments and open in the browser.

## Testing

There are no automated tests in this repository. When you build practice projects elsewhere, follow Phase 7 in the roadmap (JUnit 5, Mockito, MockMvc, integration tests, Testcontainers as appropriate).

## Project structure

| Path | Description |
| --- | --- |
| `README.md` | Main roadmap, checklist, and entry point |
| `Project Roadmap and Projects.md` | Hands-on project ideas by difficulty |
| `Recommended Learning Resources.md` | Documentation, tutorials, and optional courses |
| `Interview Preparation.md` | External interview question collections |
| `Cheatsheets.md` | Quick references and PDF links |
| `Downloadable Springboot roadmap.md` | Standalone roadmap image |
| `LICENSE` | MIT License |

## Configuration

No configuration files or environment variables apply to this documentation repository.

## Deployment

The canonical copy lives on GitHub at [vonmiller1/spring-boot-guide](https://github.com/vonmiller1/spring-boot-guide). You may fork the repository for personal notes; there is no CI/CD or container deployment defined here.

## Who this guide is for

- Developers who know little or no Java and want a structured starting point.
- Java developers moving into Spring and Spring Boot.
- Students preparing for internships, placements, or backend interviews.
- Developers who want to practice production-minded backend engineering.

## Start here

1. Review the phases below and begin with any prerequisites you have not yet covered.
2. Work through topics in order; build the suggested project before moving on.
3. Use the [project ideas](Project%20Roadmap%20and%20Projects.md) to extend your practice.
4. Keep the progress checklist and revisit topics by applying them to a project.

This is a learning guide, not a required certification path. You can use Maven or Gradle and choose PostgreSQL or MySQL; focus on understanding the concepts rather than completing every optional topic.

## Learning roadmap

### Phase 0 — Foundations

**Java:** variables, control flow, methods, arrays, object-oriented programming, exceptions, collections, generics, streams and lambdas, file I/O, concurrency basics, records, `Optional`, the `java.time` API, and JVM fundamentals.

**Supporting skills:** SQL queries, joins, indexes, transactions, and database design; HTTP methods, status codes, headers, JSON, and REST principles; Git, branches, commits, pull requests, and merge-conflict resolution; SOLID principles, composition, dependency injection, and common design patterns.

**Practice:** build a small Java command-line application and manage its source with Git.

### Phase 1 — Build tools

Learn Maven or Gradle: dependency management, plugins, build lifecycles, profiles, packaging, and executable JARs.

**Practice:** package the command-line application as an executable JAR.

### Phase 2 — Spring Core

Understand inversion of control, dependency injection, beans and their lifecycles, bean scopes, component scanning, and configuration classes.

**Practice:** create a small service and supply its dependencies through Spring.

### Phase 3 — Spring Boot

Explore Spring Initializr, auto-configuration, starter dependencies, application configuration, profiles, configuration properties, logging, and Actuator.

**Practice:** create a simple Spring Boot REST application and configure it for more than one environment.

### Phase 4 — REST APIs

Build APIs with controllers, request mappings, CRUD operations, DTOs, validation, consistent error responses, `ResponseEntity`, pagination, sorting, API versioning, and OpenAPI documentation.

**Practice:** create a Student Management API with validation and centralized exception handling.

### Phase 5 — Persistence

Use Spring Data JPA and Hibernate; map entities and relationships; write JPQL and native queries; manage transactions; and use Flyway or Liquibase for schema changes. Then study fetching, cascade behavior, the N+1 problem, query optimization, connection pooling, and optimistic and pessimistic locking.

**Practice:** build an Employee Management API backed by a relational database.

### Phase 6 — Security

Learn Spring Security, password encoding, authentication and authorization, role-based access control, and the distinction between session-based and token-based security. Explore JWT and OAuth 2.0 after understanding the fundamentals; cover CORS and CSRF in their appropriate contexts.

**Practice:** secure an API and document its authentication and authorization behavior.

### Phase 7 — Testing

Practice JUnit 5, Mockito, Spring MVC testing with MockMvc, integration testing, and Testcontainers. Choose the test scope to match the behavior being verified.

**Practice:** add unit and integration coverage to the Student Management API.

### Phase 8 — External services

Learn to make outbound HTTP calls, configure API keys safely, set timeouts, and handle retries, rate limits, and failures. Explore Spring's HTTP clients and resilience patterns such as circuit breakers.

**Practice:** build a weather-service client that handles slow or unavailable upstreams.

### Phase 9 — Containers and deployment

Learn Docker, Docker Compose, multi-stage builds, environment-based configuration, volumes, and networking. Deploy an application and understand reverse proxies, HTTPS, and domain configuration.

**Practice:** containerize and deploy the Employee Management API without committing credentials.

### Phase 10 — Architecture and production readiness

Study layered and feature-based designs, clean and hexagonal architecture, DTO-versus-entity boundaries, and modular-monolith versus microservice trade-offs. Practice logging, validation, API documentation, email and file handling, caching, and application health and metrics.

**Practice:** refactor an existing API around clear boundaries and add operational documentation.

### Phase 11 — Advanced topics

Explore these topics when you have a working foundation:

- **Messaging:** Kafka or RabbitMQ.
- **Microservices:** service boundaries, Spring Cloud, service discovery, configuration, API gateways, and OpenFeign.
- **Caching:** Redis and cache invalidation.
- **Reactive programming:** WebFlux and Project Reactor, when the use case warrants it.
- **GraphQL:** schema and API design with Spring.
- **Observability:** Micrometer, Prometheus, and Grafana.
- **CI/CD:** automated tests, builds, image publishing, and deployment pipelines.

**Practice:** split a well-understood application only when there is a clear architectural reason, then document the trade-offs.

## Project standards

For each substantial project, aim to include:

- Clear REST conventions, input validation, and consistent error handling.
- A documented API and setup instructions.
- Configuration through environment variables or a secrets manager; no committed secrets.
- Database migrations where a database is used.
- Focused unit and integration tests.
- Docker support and a repeatable local development setup.
- A Postman or Bruno collection where useful.
- A deployment or operations note, even if the project is not hosted.

Start small and add these practices as they become relevant; not every exercise needs every production feature.

## Resources in this repository

| Guide | Use it for |
| --- | --- |
| [Project ideas](Project%20Roadmap%20and%20Projects.md) | Hands-on exercises organized by difficulty |
| [Learning resources](Recommended%20Learning%20Resources.md) | Official documentation, tutorials, and books |
| [Interview preparation](Interview%20Preparation.md) | Practice question collections by topic |
| [Cheatsheets](Cheatsheets.md) | Quick references for common developer tools |
| [Downloadable roadmap](Downloadable%20Springboot%20roadmap.md) | Roadmap graphic |

## Progress checklist

- [ ] Java fundamentals, OOP, collections, exceptions, and basic concurrency
- [ ] SQL, relational modeling, joins, indexes, and transactions
- [ ] HTTP, REST, and Git collaboration
- [ ] Maven or Gradle and Spring Core
- [ ] Spring Boot configuration and REST APIs
- [ ] Validation, error handling, and API documentation
- [ ] Persistence, JPA, migrations, and query behavior
- [ ] Security fundamentals and appropriate authentication
- [ ] Unit, MVC, and integration testing
- [ ] External-service integration and failure handling
- [ ] Docker and a deployment workflow
- [ ] Architecture, logging, and operational readiness
- [ ] Advanced topics selected for a project or career goal

## Roadmap graphic

![Spring Boot backend developer roadmap](https://github.com/user-attachments/assets/f79841ce-ab40-404b-b88b-e46131a3c0eb)

The roadmap is a guide, not a substitute for the official documentation. Thanks to Amigoscode for the original roadmap inspiration, and to VenkatMal Reddy Desai for the introduction to the Java developer environment.

## Contributing

1. Fork the repository and create a feature branch from `main`.
2. Keep edits focused; prefer updating links and clarity over large rewrites unless accuracy requires it.
3. Use clear, imperative commit messages (for example, `docs(readme): clarify Phase 5 persistence topics`).
4. Open a pull request describing what you changed and why.
5. Do not commit secrets, API keys, or personal data in examples.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
