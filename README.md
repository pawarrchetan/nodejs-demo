# Project Title

Demo nods.js app
The project has files for creating a containerized node.js app which give sinformation about a few types of sharks.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

* A sudo user on your server or in your local environment.
* Docker.
* Node.js and npm.
* A Docker Hub account.

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be


1. Clone this repository in your system
    ```
    git clone https://github.com/pawarrchetan/nodejs-demo.git
    ```
2. You have multiple ways to run the application.
    1. Create docker image using the `Dockerfile` and run the application locally on your machine.
        ```
        docker build -t your_dockerhub_username/nodejs-image-demo .
        docker run --name nodejs-image-demo -p 80:8080 -d your_dockerhub_username/nodejs-image-demo 
        ```
    2. Create the docker image using the `Dockerfile` and push the image to a Docker Hub repository or a Image repositry of your choice. 
        ```
        docker build -t your_dockerhub_username/nodejs-image-demo .
        docker login -u your_dockerhub_username -p your_dockerhub_password
        docker push your_dockerhub_username/nodejs-image-demo
        ```

With your container running, you can now visit your application by navigating your browser to http://your_server_ip or localhost. 

You will see your application landing page:

![Application Page ](https://assets.digitalocean.com/articles/docker_node_image/node_image_landing.png)

## Built With

* [Nodejs](https://nodejs.org/en/docs/) - The web framework used
* [NPM](https://www.npmjs.com/) - Dependency Management

## Contributing

Please read [CONTRIBUTING.md](https://github.com/pawarrchetan/nodejs-demo/blob/master/contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Chetan Pawar** - *Initial work*
