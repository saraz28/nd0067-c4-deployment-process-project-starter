# Pipeline Process

## Overview

The CI/CD pipeline automates the process of building, testing, and deploying our application using AWS services.

In this project we use **CirclCi** platform to do auomations of our application. it represents the overall flow of the tasks that need to be executed for a project. Within a pipeline, there are jobs, workflows, and steps that define the process.

### 1. first step

Setup an account integrated with github each time a new commit is pushed to the repository A pipeline starts to do the job. A job is a collection of steps to perform different tasks for example:

- **build:** To compile or package the code.
- **test:** To run unit tests, integration tests, or other types of tests.
- **deploy:** To deploy the application to a staging or production environment.

### 2. second step

Is to set environment variables for use in jobs. The following is the variables used in our project.

- POSTGRES_DB
- AWS_BUCKET
- AWS_REGION
- AWS_PROFILE
- JWT_SECRET
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
