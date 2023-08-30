# Project Description

This repository is developed using Nest.js.

## Google API Key

To use this project, you need to generate an API Key in the Google Console and activate the `Google Maps API` service.

## Running the Application

To run the application, follow these steps:

1. Start the application using Docker Compose:

    ```bash
    docker-compose up
    ```

2. In another terminal, enter the Docker container:

    ```bash
    docker compose exec app bash
    ```

3. Configure the initial dependencies (inside the Docker container):

    ```bash
    npm install
    npx prisma generate
    ```

4. Run the application (inside the Docker container):

    ```bash
    npm run start:dev
    ```

5. Access the application at http://localhost:3000/routes.

There is a file in the root of the Nest.js project named `api.http` that you can use to test the application with the [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) plugin for VSCode. When you send data in the request, Nest.js will consume the message and display it in the console.

## Installation

```bash
$ npm install


# Development mode
$ npm run start

# Watch mode
$ npm run start:dev

# Production mode
$ npm run start:prod


# Unit tests
$ npm run test

# End-to-end (e2e) tests
$ npm run test:e2e

# Test coverage
$ npm run test:cov
