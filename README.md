## Overview

An example project to demonstrate:

* how to create a Spring Boot REST API
* how to run Spring Boot in Docker and publish to Docker Hub

## Pre-requisites

* JDK 8+
* Docker

## Building

### Testing

`./gradlew test`

### Building (no tests)

`./gradlew assemble`

### Building (with tests)

`./gradlew build`

### Running in Docker

`./gradlew assemble docker dockerRun`

### Stopping Docker container

`./gradlew dockerStop`

### Deploying to AWS

`./gradlew awsCfnMigrateStack awsCfnWaitStackComplete -PsubnetId=<your-subnet-id> -Pregion=<your-region>`

### Deleting AWS deployment

`./gradlew awsCfnDeleteStack awsCfnWaitStackComplete`