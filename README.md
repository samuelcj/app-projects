# app-projects
This repository contains three sub-modules that represent the three Application Projects, demonstrating Build and Package Management Tools.

- **Project 1**: Java Gradle Application (`java-gradle-app`)
- **Project 2**: Java Maven Application (`java-maven-app`)
- **Project 3**: Node.js Application (`nodejs-app`)

Each project has its specific build instructions, deployment steps, and additional configurations. Below are the unified details for each project.

---

## Project 1: Java Gradle App

This project is built using Gradle.

### Build the Project

To build the project, use the following command:

```bash
./gradlew build
```

### Build Docker Image

To create a Docker image named `java-app`, execute the following command from the root directory:

```bash
docker build -t java-app .
```

### Push Docker Image to Repository

Tag the Docker image and push it to your repository:

```bash
docker tag java-app demo-app:java-1.0
```

## Project 2: Java Maven App

This project is built using Maven.

### Build the Project

To build the project, use the following command:

```bash
mvn clean install
```

### Run Tests

To run the tests in the project, use:

```bash
mvn test
```

### Dockerization

You can build a Docker image for this project similarly. For example, to build the image named `maven-app`, you can use:

```bash
docker build -t maven-app .
```

---

## Project 3: Node.js App

This project is part of the DevOps bootcamp exercise for **Cloud Basics**.

### Testing the Project

The project uses the `jest` library for testing. There is one test (`server.test.js`) that verifies the existence of the main `index.html` file in the project.

#### To run the tests:

1. Install dependencies if not already installed:

   ```bash
   npm install
   ```

2. Run the test:

   ```bash
   npm run test
   ```

#### Failing Tests

To see a failing test, you can remove or rename `index.html` and re-run the tests.

---

## General Instructions

- Each project may require specific setup steps before running the above commands. Make sure to install dependencies as needed (e.g., using `npm install` for Node.js, or `mvn install` for Maven-based Java projects).
- Ensure that Docker is installed and running if you plan to build Docker images for any of the projects.
- For any issues related to specific technologies, please refer to the respective project documentation.

---

Feel free to contribute to any of the individual projects by creating an issue or submitting a pull request. Enjoy building!


