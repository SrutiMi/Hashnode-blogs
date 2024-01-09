---
title: "The Reason Why We Use Different Tools In DevOps"
datePublished: Wed Jan 03 2024 08:19:53 GMT+0000 (Coordinated Universal Time)
cuid: clqxicn7i000508juf9tph593
slug: the-reason-why-we-use-different-tools-in-devops
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1704269899298/79d72ab7-f01c-4148-8c82-9a23b50c1614.webp
tags: devops

---

You've probably heard of DevOps tools like Git, Docker, Kubernetes, Ansible, and more. It can be not very clear to figure out why there are so many different tools in DevOps. But don't worry, I'm here to help! Let me explain it to you in a way that's easy to understand.

So, let's say you've built a cool application and now you want to share it with the world. You'll need to host your app in a data center, either on a physical server or a virtual machine in the cloud.

Now, there are two terms you should remember - development environment and production environment. Think of your laptop as the development environment where you've created the code for your app. And the production environment is the server where you'll host your app.

But there's a catch! The code you've written can't be understood by the end user. It needs to be converted into a binary or executable form before it can be deployed. This process is called "building the code". Once the code is built, the executable is moved to the production environment, i.e., the server, where it's run. This stage is known as the "deploy stage".

Imagine your application has become very popular and you need to add more features. You have hired different developers who are working on their respective laptops. All developers are working on the same codebase and they need to show their changes in the code in the same place. This is where Git and GitHub come in. GitHub is a cloud-based platform that serves as a central location for all code. We can push our code to it. Git is a command-line tool that enables versioning of code and collaboration between multiple developers. With Git and Github, the development issue is solved.

When it comes to producing our application, we sometimes run into a bit of a problem. You see, just building on one person's laptop isn't enough to ensure that everyone is up to date with the latest changes. That's why we move the build operation to a dedicated server, where we manually copy the latest version of the code and build it before deploying it into production.

But sometimes, pushing new builds can be risky because it might introduce new bugs. So, we need to manually test it in a separate test environment before copying the executable to the production environment and deploying it. Unfortunately, this takes a lot of time, and even minor changes can take days to implement.

That's where our CI/CD (continuous integration and continuous delivery/deployment) tools come in handy! We use tools like GitHub Actions, GitLab or Jenkins to automate these manual tasks and build a pipeline. Every time code is pushed, it's automatically pulled from the GitHub repository to the build server. The executable is then automatically moved to the test server and after it's been successfully tested, it's automatically moved to the production server and deployed.

We're still facing a few issues with the dependencies and libraries required for our applications to run. It can be quite challenging to configure these dependencies on all servers, and if we miss something, it can lead to unexpected outcomes on different systems.

But, we have a solution! We use containers to package the application and its dependencies together. That way, we don't have to worry about configuring dependencies on each system. All other systems can run the container from the same image, which is super convenient.

Containers also help to isolate processes. Each container is an isolated instance, which means we can run multiple containers, each with its separate instance of the application on the same server. We use Docker to work with these containers, and it's been a real lifesaver.

So right now we have just one server that's taking care of all our users, but we're growing so fast that we need to add more servers to handle the load. The tricky part is making sure that we can spin up more containers automatically when we get busy, and shut them down when things calm down. But don't worry! This is where platforms like Kubernetes come in. They help us manage all our containers in a way that's smart, scalable, and automated. Cool, huh?

Setting up and configuring servers in a cluster can be a bit of a challenge. Each new server needs to be set up just like the others, with the right resources and operating system. But don't worry, there are tools like Terraform that can help! Terraform automates the process of setting up and configuring servers, no matter what cloud platform they're on. And because the configuration is written in code, it's called "infrastructure as code". Once your servers are up and running, you can use Ansible to automate their configuration and make sure everything stays in tip-top shape.

Now, to keep your servers running smoothly, you'll want to monitor them and catch any issues before they become big problems. That's where Prometheus comes in. Prometheus lets you keep an eye on important metrics like CPU usage, memory consumption, and running processes. With this information, you can identify any processes that are using too many resources and take action to prevent any issues.

I hope you've got a good grasp on why we use different tools in DevOps. Let me know if you have any questions or if there's anything else I can help you with!