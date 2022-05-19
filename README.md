In this project, I have tried to simulate a CI/CD pipeline for a node.js application using the Jenkins integration tool. For this i had to use different applications/software’s and set of tools which are listed and discussed below:

<h1> AWS EC2 Cloud Instance </h1>
I used AWS EC2 Cloud instance to deploy our node.js source code. The same instance is used to install the Jenkins Integration tool, Docker Engine, Docker-Compose for running the CI/CD from Jenkins to deploy the node.js application over the same instance.

<h1> Ubuntu OS on EC2 Instance </h1>	
The unix based Ubuntu OS is chosen to deploy the application and the tools to be used for the CI/CD. The AWS EC2 Cloud instance is loaded with Ubuntu image at the time of spinning the EC2 instance.

<h1> Jenkins Integration Tool	</h1>
The Jenkins is most common widely used integration tool for deploying CI/CD pipelines for setting up DevOps lifecycle. I  have installed this Jenkins on the Ubuntu 20.04 instance to setup Continuous Integration/Continuous Delivery pipelines for our node.js application automated deployment.

<h1> Docker Engine </h1>
Docker is the most commonly used containerization tool these days. As you all know about containerization so I wont need to discus it here, you will find several introductory lectures about this over internet. In short containerization enables us to run our application in isolated environment and is very helpful in micro services architecture. Here I have installed the docker-engine on Ubuntu instance to deploy our application in a containerized environment.

<h1> Sample Application </h1>
The sample application used in this example is node.js application which is simple login app with mysql database. The sample node.js applictaion is written in package.json file and is able to perform two function, one is login and another is registering the user. 

I have deployed this application using the Docker containers, there are two services deployed in separate containers for this node.js application, one is MySQL database to register the users and authenticate the user login and the other is the node.js application itself which is using the node package manager running.

In this solution, we have demonstrated how the push event in central repo trigger the test build and upon successful test results, the build is deployed in staging environment from where the build could finally be deployed in production environment.

