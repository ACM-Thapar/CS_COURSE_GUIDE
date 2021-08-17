<div align = "center">

  # Devops Guide 


<p float="left" align="middle">
<img height=100px style="margin:7.5px" src= "https://www.vectorlogo.zone/logos/docker/docker-official.svg">

<img height=100px style="margin:7.5px" src= "https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg">

<img height=100px style="margin:7.5px" src= "https://www.vectorlogo.zone/logos/travis-ci/travis-ci-icon.svg">

<img height=100px style="margin:7.5px" src= "https://www.vectorlogo.zone/logos/nginx/nginx-ar21.svg">

<img height=100px style="margin:7.5px" src= "https://www.vectorlogo.zone/logos/amazon_aws/amazon_aws-ar21.svg">
</p>
</div>

**Pre-requisites**
- Good understanding of web development concepts and workflow.
- Comfortable with command line actions and familiarity with source code version control systems such as Git.
- Curiosity to learn new technologies, offer novel solutions and recommendations and be adaptive to face challenges.
- Grasp of networking concepts and tools.

### Table of Contents
- [What is DevOps?](#what-is-devops)
    - [DevOps Practices](#devops-practices)
        - [Continuous Development](#1-continuous-development)
        - [Continuous Integration](#2-continuous-integration-ci)
        - [Continuous Delivery](#3-continuous-delivery-cd)
        - [Continuous Deployment](#4-continuous-deployment)
        - [Continous Testing](#5-continuous-testing)
        - [Continuous Monitoring](#6-continuous-monitoring)
        - [Infrastructure as Code](#7-infrastructure-as-code)
        - [Microservices](#8-microservices)
- [How to begin](#how-to-begin)
    - [Basic Concepts](#basic-concepts) 
        - [Containerization](#containerization)
        - [OSI Network Model](#osi-network-model)
        - [TCP/IP Network Model](#tcpip-network-model)
        - [Transport Protocols](#transport-protocols)
        - [Beginner Devops Engineering Concepts](#beginner-devops-engineering-concepts)
- [Docker](#docker)
    - [What is Docker?](#what-is-docker)
- [Kubernetes](#kubernetes)
    - [What is Kubernetes?](#what-is-kubernetes)
- [Travis CI](#travis-ci)
    - [What is Travis CI?](#what-is-travis-ci)
- [Nginx](#nginx)
    - [What is Nginx?](#what-is-nginx)
- [Amazon Web Services](#amazon-web-services)
    - [What is Amazon Web Services?](#what-is-amazon-web-services)
- [Recommended Courses](#recommended-courses)
- [Extensive Roadmap](#extensive-roadmap)

## What is DevOps?
<div align="center">
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmiro.medium.com%2Fmax%2F3964%2F1*9pVLG4BzEWIcMnfhFp9ULQ.png&f=1&nofb=1" height="220" width="400" alt="Devops">
</div>

- DevOps can be explained simply as operations working together with engineers to get things done faster in an automated and repeatable way.
> You can ask 10 people for a definition of DevOps and likely get 10 different answers.
- The term DevOps is a combination of two words namely Development and Operations. DevOps is a practice that allows a single team to manage the entire application development life cycle, that is, development, testing, deployment, and monitoring.
- The ultimate goal of DevOps is to decrease the duration of the system’s development life cycle while delivering features, fixes, and updates frequently in close synchronization with business objectives.
- DevOps is a software development approach with the help of which you can develop superior quality software quickly and with more reliability. It consists of various stages such as continuous development, continuous integration, continuous testing, continuous deployment, and continuous monitoring.

### DevOps Practices
#### 1. Continuous Development
- This is the phase that involves planning and coding of the software. You decide the project vision during the planning phase and the developers begin developing the code for the application.

<div align="center">
<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2020/01/download.png" height="200" width="300" alt="Continuous Development">
</div>

#### 2. Continuous Integration (CI)
- Continuous Integration (CI) is a DevOps practice in which developers frequently merge their code changes to the central repository. Then, the code is built automatically and automated tests are run against the built code.

#### 3. Continuous Delivery (CD)
-  Continuous Delivery (CD) is the automation of steps to safely get changes into production. Where Continuous Deployment focuses on the actual deployment, Continuous Delivery focuses on the release and release strategy.

#### 4. Continuous Deployment 
- This is the stage where you deploy the code on the production servers. It is also important to ensure that you correctly deploy the code on all the servers.

<div align="center">
<img src="https://www.redhat.com/cms/managed-files/styles/wysiwyg_full_width/s3/ci-cd-flow-desktop_0.png?itok=QgBYmjA2" height="150" width="600" alt="Continuous Deployment">
</div>

#### 5. Continuous Testing
- This is the stage where you test the developed software continuously for bugs using automation testing tools.
- The Continuous Testing practice helps to identify potential risks as early as possible in all stages of the development lifecycle to minimize the impact on end-users.

#### 6. Continuous Monitoring
- This is a very critical stage of the DevOps life cycle where you continuously monitor the performance of your application. Here you record vital information about the use of the software. You then process this information to check the proper functionality of the application. You resolve system errors such as low memory, server not reachable, etc in this phase.

#### 7. Infrastructure as Code (IaC)
- IaC is a DevOps practice that involves the use of a configuration management tool to manage the infrastructure.
- Infrastructure as Code (IaC) is a practice where infrastructure—virtual machines, load balancers, networks, etc.—are configured and managed using code rather than manually setting up and managing those resources. This has become an essential DevOps practice in organizations who specifically have moved to cloud platforms.

#### 8. Microservices
- A microservice is a small, independent, self-contained application that is designed to be deployed in a distributed environment.
- Unlike in traditional monolithic architectures, in microservices architecture, a single application is built as a set of small services or components. These separate services have their own functionality and their communication happens through a lightweight interface or an API.


## How to begin 

### Basic Concepts

##### - [Containerization](https://www.youtube.com/watch?v=0qotVMX-J5s)
##### - [OSI Network Model](https://www.youtube.com/watch?v=dV8mjZd1OtU)

##### - [TCP/IP Network Model](https://www.youtube.com/watch?v=F5rni9fr1yE)

##### - [Transport Protocols](https://www.youtube.com/watch?v=37AFBZv4_6Y)

##### - [Beginner Devops Engineering Concepts](https://www.freecodecamp.org/news/devops-engineering-course-for-beginners/)
 

## Docker
### What is Docker?
- Docker is an open-source tool designed to help in creating containers and container-based applications in the form of docker containers.
- In other words, it is a containerization platform that simplifies the building, shipment, and running application.
- Docker streamlines the development lifecycle by allowing developers to work in standardized environments using local containers which provide your applications and services. Containers are great for continuous integration and continuous delivery (CI/CD) workflows.

## Kubernetes
### What is kubernetes?
- Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation.
- Kubernetes orchestrates clusters of virtual machines and schedules containers to run on those virtual machines based on their available compute resources and the resource requirements of each container. 
- Containers are grouped into pods, the basic operational unit for Kubernetes and those pods scale to your desired state.

## Travis CI
### What is Travis CI?
- Travis CI is a hosted, distributed continuous integration service used to build and test projects hosted at GitHub. 
- Travis CI was the first CI as a Service tool. It introduced a new approach to building code in the cloud. This CI tool allows the user to sign up, link their repository, build, as well as test their apps. Travis CI tool can easily integrate with the common cloud repositories like GitHub and Bitbucket.

## Nginx
### What is Nginx?
- Nginx is open source software for web serving, reverse proxying, caching, load balancing, media streaming, and more. It started out as a web server designed for maximum performance and stability.
-In addition to its HTTP server capabilities, Nginx can also function as a proxy server for email (IMAP, POP3, and SMTP) and a reverse proxy and load balancer for HTTP, TCP, and UDP servers.
- The goal behind Nginx was to create the fastest web server around.

## Amazon Web Services
### What is Amazon Web Services?
- Amazon Web Services(AWS) is a cloud service from Amazon, which provides services in the form of building blocks, these building blocks can be used to create and deploy any type of application in the cloud.
- These services or building blocks are designed to work with each other, and result in applications that are sophisticated and highly scalable.
- It provides scalable and cost-effective cloud computing solutions.
- AWS is a broadly adopted cloud platform that offers several on-demand operations like compute power, database storage, content delivery, etc., to help corporates scale and grow.


## Recomended Courses
- [Docker and Kubernetes: The Complete Guide](https://www.udemy.com/docker-and-kubernetes-the-complete-guide/)]
    - This course provides you an insight to the world of docker, kubernetes and how to use them. It also introduces the concepts of containerization and continuous integration along with Travis CI, Nginx and Amazon Web Services.

## Extensive Roadmap
- [DevOps: The Complete Roadmap](https://roadmap.sh/devops)