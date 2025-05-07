# AutoAPI-TicTacToe-Agent

## Overview
The AutoAPI-TicTacToe-Agent leverages prompt engineering techniques to create the project for tic-tac-toe. The `.github/prompts` folder contains predefined prompt templates that guide the agent's behavior and responses. These prompts are designed to handle various API interaction scenarios, ensuring flexibility and adaptability in diverse use cases.

This tool helps with creating and managing APIs, containerizing to deploy, making it easier to build and maintain software applications. 

## Features

- **Code Generation**: The agent can create APIs based on user-defined specifications and requirements in Tictactoe_prompts.md.
- **Dependency Injection**: The agent can inject dependencies into the codebase, ensuring that all necessary libraries and frameworks are included for the application to function correctly using pyproject_prompts.md.
- **Containerization**: The agent can containerize applications using Docker, making it easier to deploy and manage software in different environments using docker_prompts.md.
- **Summary Generation**: The agent can generate a README.md file for the project, providing essential information about the application, its usage, and its dependencies and how to deploy it locally as well as in a docker container using readme_prompts.md.

## Prerequisites

- VSCode
- Active GitHub copilot account
- Optional: Azure AI account for additional features and capabilities.

## Usage:

1. Clone the repository:
   ```bash
   git clone
    ```

2. Navigate to the project directory and open GitHub copilot:
   ```Coplilot
    Add the tictactoe_prompts.md file to the github copilot context
    Type: Run tictactoe_prompts.md -- send
    ```

3. Follow the prompts to create the API for tic-tac-toe.
4. Once the API is created, you can use the pyproject_prompts.md file to inject dependencies into the codebase in the similar way.
5. After injecting dependencies, use the docker_prompts.md file to containerize the application.
6. Finally, use the readme_prompts.md file to generate a README.md file for the project.
7. Follow the instructions in the README.md file to run the application locally and in a Docker container.



