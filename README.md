# Jenkins Basics

A beginner-friendly guide to understanding and using Jenkins for Continuous Integration and Continuous Deployment (CI/CD).

---

## Table of Contents
- [What is Jenkins?](#what-is-jenkins)
- [Key Features of Jenkins](#key-features-of-jenkins)
- [Jenkins Architecture](#jenkins-architecture)
- [Basic Jenkins Terminology](#basic-jenkins-terminology)
- [Typical Jenkins Workflow](#typical-jenkins-workflow)
- [Best Practices](#best-practices)

---

## What is Jenkins?

Jenkins is an open-source automation server used to automate parts of software development like building, testing, and deploying applications.  
It helps implement Continuous Integration and Continuous Delivery (CI/CD) pipelines.

<p align="center">
  <img src="https://www.jenkins.io/images/logos/jenkins/jenkins.png" alt="Jenkins Logo" width="150" />
</p>

---

## Key Features of Jenkins
> **Open Source**  
> Free to use with a large community.

> **Extensible**  
> Supports 1,800+ plugins for building, deploying, and automating.

> **Distributed Builds**  
> Supports Master-Agent architecture to manage multiple builds across different machines.

> **Easy Installation**  
> Simple installation through `.war` files, Docker images, or package managers.

> **Rich UI and REST APIs**  
> Provides a web-based interface and APIs to manage Jenkins.

---

## Jenkins Architecture

Jenkins follows a **Master-Agent** architecture.

> **Master (Controller)**  
> - Orchestrates the tasks.  
> - Manages project configuration.  
> - Assigns builds to agents.

> **Agent (Node)**  
> - Executes the tasks like building, testing, and deployment.

> **Executor**  
> - A slot on the agent where a build runs.

---

## Basic Jenkins Terminology

> **Job / Project**  
> A task like building code, running tests, or deploying an application.

> **Build**  
> The actual execution instance of a job.

> **Pipeline**  
> Defines the entire build, test, and deploy workflow as code.

> **Plugin**  
> Extensions that add new features to Jenkins.

> **Workspace**  
> The directory where Jenkins stores files related to a job.

---

## Typical Jenkins Workflow

1. Developer pushes code to a Git repository (GitHub, GitLab, Bitbucket).
2. Jenkins detects the change via Webhooks or Poll SCM.
3. Jenkins pulls the updated code.
4. Jenkins builds the code.
5. Jenkins runs tests.
6. Jenkins deploys the build to a server or cloud.

---

## Best Practices

> **Use Pipelines as Code**  
> Define pipelines in `Jenkinsfile` for better version control.

> **Limit Plugins**  
> Only use necessary plugins to keep Jenkins lightweight and secure.

> **Secure Jenkins**  
> Use authentication, authorization, and always configure security settings properly.

> **Use Backup and Restore Plugins**  
> Regularly back up Jenkins configurations and jobs.

> **Use Distributed Builds**  
> Set up multiple agents to distribute the load and speed up builds.

---

## Useful Resources
- [Official Jenkins Documentation](https://www.jenkins.io/doc/)
- [Jenkins GitHub Repository](https://github.com/jenkinsci/jenkins)
- [Jenkins Plugins Index](https://plugins.jenkins.io/)
