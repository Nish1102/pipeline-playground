# Jenkins Pipeline Example

This repository contains a basic example of a Jenkins pipeline script with stages for HelloWorld, Build, Test, and Deploy.

## Getting Started

These instructions will help you set up and run the Jenkins pipeline on your local or Jenkins server.

### Prerequisites

- Jenkins server (configured with necessary plugins)
- Docker (if using the Docker container in the Test stage)

### Running the Pipeline

1. Clone this repository:

    ```bash
    git clone https://github.com/nish1102/jenkins-pipeline-example.git
    ```

2. Open Jenkins and create a new pipeline job.

3. Configure the pipeline to point to the Jenkinsfile in this repository.

4. Build the pipeline.

## Pipeline Stages

### HelloWorld

Prints "Hello, World!" to the console.

### Build

Placeholder for your build steps.

### Test

Runs a simple test inside a Docker container using Node.js.

### Deploy

Placeholder for your deployment steps.

## Post-Build Actions

- `always`: Echoes a message that will always be executed.
- `success`: Echoes a message if the build succeeds.
- `failure`: Echoes a message if the build fails.

## Contributing

Feel free to contribute by opening issues or pull requests. Your feedback is appreciated!

