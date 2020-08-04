# Code

## Context

* These notes are part of a broader set of [principles](../principles.md)

## Principles

* Everything (including infrastructure) should be created by code
* All code is treated the same (e.g. application code, infrastructure code, test code, etc)
* All code is peer-reviewed and tested
* All code is version controlled
* Code changes should be automatically checked for code quality using tools like [SonarQube](https://www.sonarqube.org) (as well as via IDE plugins)
* Code should be automatically scanned for secrets or other sensitive data using tools like [AWS Macie](https://aws.amazon.com/macie/)
* Prefer convention over configuration as it lowers down the complexity of the software
* Prefer well structured and expressive code over extensive documentation as it is the single source of truth
* Always design the interface prior to the implementation and define vocabulary to make it coherent - that includes not only the interfaces (e.g. REST API) on the edge of a system but components, classes, as well as method signatures
* Adopt consumer-driven contract testing to stabilise interface
* Adopt test-first approach to minimise waste and increase cohesion of the code
* Follow the clean code practices across the whole software stack, see [Clean Code](https://www.oreilly.com/library/view/clean-code/9780136083238/) and [Clean Architecture](https://www.oreilly.com/library/view/clean-architecture-a/9780134494272/)
