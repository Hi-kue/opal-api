# Opal API - Books API

## Description

Opal API is a simple Rest API, made with Quarkus and JPAStreamer that allows you to manage
categories of books, and their respective ratings and reviews within their categories. The 
API provides functional CRUD operations for categories, individual books, and is documented
using Swagger UI.

## Table of Contents

- [Setup](#setup)


## Setup

### Running the Application in Dev Mode

You can run the application in dev mode, that enables live coding using:
```shell script
./mvnw compile quarkus:dev
```

> **_NOTE:_**  Quarkus now ships with a Dev UI, which is available in dev mode only at http://localhost:8080/q/dev/.

### Packaging and Running the Application

To package the application, simply use:
```shell script
./mvnw package
```

This will produce a `quarkus-run.jar` file in the `target/quarkus-app/` directory. The 
application is now runnable using the following:
1. `java -jar target/quarkus-app/quarkus-run.jar`.

If you are looking to build an _über-jar_, execute the following command:
```shell script
./mvnw package -Dquarkus.package.jar.type=uber-jar
```

The application will be packaged as an _über-jar_ can be run using the following:
1. `java -jar target/*-runner.jar`.


### Creating a Native Executable

You are able to create a native executable as well using:
```shell script
./mvnw package -Dnative
```

Or, if you don't have GraalVM installed, you can just run the native executable
build in a container using:
```shell script
./mvnw package -Dnative -Dquarkus.native.container-build=true
```

Executing can be done using the following:
1. `./target/opal-api-1.0.0-SNAPSHOT-runner`

### Related Guides

- REST resources for Hibernate ORM with Panache ([guide](https://quarkus.io/guides/rest-data-panache)): Generate Jakarta REST resources for your Hibernate Panache entities and repositories
- JPAStreamer ([guide](https://quarkiverse.github.io/quarkiverse-docs/quarkus-jpastreamer/dev/)): Express your Hibernate queries as standard Java Streams
- SmallRye OpenAPI ([guide](https://quarkus.io/guides/openapi-swaggerui)): Document your REST APIs with OpenAPI - comes with Swagger UI
- REST Jackson ([guide](https://quarkus.io/guides/rest#json-serialisation)): Jackson serialization support for Quarkus REST. This extension is not compatible with the quarkus-resteasy extension, or any of the extensions that depend on it
- Hibernate ORM with Panache ([guide](https://quarkus.io/guides/hibernate-orm-panache)): Simplify your persistence code for Hibernate ORM via the active record or the repository pattern
- JDBC Driver - MySQL ([guide](https://quarkus.io/guides/datasource)): Connect to the MySQL database via JDBC

### Getting Started

To get started with this repository, you can clone it to your local machine using 
the following command:
```shell script
git clone https://github.com/Hi-kue/opal-api.git
```

After cloning, you should navigate to the root directory of the project and run:
```shell script
./mvnw compile quarkus:dev
```

This will setup the application in dev mode, which provides live reloading functionality.

### Testing

## License

## Authors