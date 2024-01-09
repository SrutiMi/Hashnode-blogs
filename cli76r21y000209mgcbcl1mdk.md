---
title: "Sailing into the World of Docker"
datePublished: Sun May 28 2023 08:55:31 GMT+0000 (Coordinated Universal Time)
cuid: cli76r21y000209mgcbcl1mdk
slug: sailing-into-the-world-of-docker
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1685262998009/0f2f27a3-47b7-4d86-9e7c-278173635b74.webp
tags: docker

---

Whether you're involved in web development or DevOps, you've likely come across the term "Docker." Docker is a technology that runs containers, but you might be wondering what exactly containers are and why containerization is important. So let's first understand the concepts of images, containers, and the significance of containerization.

### Images

In Docker, an image is like a template or blueprint (similar to a class) used to create containers. Images are made up of multiple layers that are stacked on top of each other and represented as a single object. It consists of everything required for an application to run such as an operating system (OS) filesystem, along with the application code and all its necessary dependencies.

We store images in centralised places called registries, for example -Docker Hub, which makes it easy to share and access them.

### Containers

In the past, servers could only handle one application at a time, which resulted in wasted resources. Then, virtual machines (VMs) came along, allowing multiple applications to run on a single server. However, VMs required their own operating system (OS), which consumed more resources and caused slower performance. To solve this, containers were introduced.

Containers are similar to VMs, but they work differently. They share the host server's OS, which means they don't need to carry their OS with them. This makes them faster to start and more efficient in using resources. Containers are designed to run a single application or service, so they only need the specific code and dependencies required for that particular app. We can say that a container is the runtime instance of an image.

### What is docker?

Docker is an open-source platform that allows us to automate the deployment, scaling, and management of applications using containerization. It provides a set of tools and technologies that make it easier to create, distribute, and run these containers.

### Some Basic docker commands:

* `docker images`: to check the existing image on the system.
    
* `docker pull <image name>`: to pull an image from a remote repository
    
* `docker run <name>`: to run the image in a container
    
* `docker ps`: to see which images are running
    
* `docker stop <container _ ID>` : to stop a container
    
* `docker logs <container_ID>`: to see the logs of a container
    
* `docker run -p <host port>:<container port>`: to map ports between the host machine and the container. For example -if we want to run a container and map the host port 8080 to the container's port 80, the command will be 'docker run -p 8080:80'.This will make the container's application accessible on the host machine at [`http://localhost:8080`](http://localhost:8080)`.`
    
* `docker build` : Allows to build image from a dockerfile.
    

### About dockerfile:

A Dockerfile is a text file that contains a set of instructions used to build a Docker image. It serves as a recipe or blueprint for creating a containerized application.

* The dockerfile starts with the '`FROM`' instruction. This specifies the base layer of the image.
    
* It has a '`LABEL`' to specify the maintainer of the image.
    
* '`RUN`' instruction is used to execute commands during the image-building process. It allows us to run any valid command inside the container(or image)being built.
    
* The '`COPY`' instruction adds files into the image as a new layer. It is used to copy the application code into an image.
    
* '`EXPOSE`' documents the network port that the application uses. This adds image metadata and not an image layer.
    
* '`ENTRYPOINT`' instruction is used to set the main application that the image (container) should run. This is added as metadata and not an image layer.
    

### Creating a docker image using dockerfile:

First write a simple Java program as follows :

![Java program](https://cdn.hashnode.com/res/hashnode/image/upload/v1685259992396/4236793a-0648-4a01-ae3e-6e70cdd28e08.png align="center")

Now in the same folder create a file named 'dockerfile'. In the dockerfile write the following instructions :

```plaintext
#using java image as the base image
FROM openjdk:11

#Setting the working directory inside the container
WORKDIR /app


COPY demo.java ./
 
#compiling the java code 
RUN javac demo.java

CMD ["java","demo"]
```

In the above Dockerfile, the instructions :

1. `FROM openjdk:11`: This specifies that the base image for the Docker image is the OpenJDK 11 image. This base image contains the Java Development Kit (JDK) and provides the necessary environment to run Java applications.
    
2. `WORKDIR /app`: This sets the working directory inside the container to `/app`.
    
3. `COPY` [`demo.java`](http://demo.java) `./`: This copies the [`demo.java`](http://demo.java) file from the local directory (where the Docker build command is executed) to the `/app` directory inside the container. The `./` refers to the current directory where the Dockerfile is located.
    
4. `RUN javac` [`demo.java`](http://demo.java): This runs the `javac` command to compile the [`demo.java`](http://demo.java) file inside the container.
    
5. `CMD ["java", "demo"]`: This sets the command that will be executed when the Docker container starts. In this case, it runs the `java` command with the argument `demo`. The `java` command launches the JVM, and `demo` refers to the compiled Java class (`demo.class`) that was generated by the previous `javac` command.
    

Now in the console run the following commands

1. ```plaintext
     docker build -t demo .
    ```
    
    This command instructs Docker to build a Docker image based on the Dockerfile located in the current directory (`.`) The resulting image will be tagged as `demo`.
    
2. ```plaintext
     docker run demo
    ```
    
    This command runs a Docker container using the image with the name `demo`.
    

If the image is created properly you will see `Hello World` printed in the console.

If you face any problems refer to: [demo-docker](https://github.com/SrutiMi/demo-docker)

---

I hope this blog has provided you with a good understanding of Docker and its significance in the world of software development. Now, it's time for you to dive in, experiment with Docker, and unleash its potential in your own projects.

If you have any questions or want to share your experiences with Docker, feel free to leave a comment below.