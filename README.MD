# Team Manager

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Docker
- Docker Compose
- Git

## Quick Start

1. **Clone the Repository**

    Clone this repository and its submodules using the following command:

    ```bash
    git clone --recurse-submodules https://github.com/Naofel-eal/Team-Manager
    ```

    If you don't want to manually rebuild the projects, you can just use the following command:  
     ```bash
    git clone https://github.com/Naofel-eal/Team-Manager
    ```

    And if you've already cloned the repository without the submodules and you need it, you can fetch them by running:

    ```bash
    git submodule update --init --recursive
    ```

    To update the images with a newest version of the game you can use the following commands:
    ```bash
    docker compose pull
    docker compose up -d --remove-orphans
    docker image prune
    ```

2. **Launch with Docker Compose**

    Navigate to the root of the Motus project where the `docker-compose.yml` file is located, and run the following command:

    ```bash
    docker-compose up
    ```

    This command will pull the necessary Docker images from Docker Hub and start the containers for the Angular frontend, Spring Boot backend, and PostgreSQL database.

3. **Access the Application**

    Once all containers are up and running, you can access the Motus game application by opening a web browser and navigating to:

    ```
    http://localhost
    ```