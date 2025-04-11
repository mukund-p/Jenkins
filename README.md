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
- [References](#references)
- [License](#license)

---

## What is Jenkins?

Jenkins is an open-source automation server used to automate parts of software development like building, testing, and deploying applications.  
It helps implement Continuous Integration and Continuous Delivery (CI/CD) pipelines.

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/Jenkins_logo.svg/320px-Jenkins_logo.svg.png" alt="Jenkins Logo" width="110" />
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

> **Pipeline**  
> A suite of plugins that supports integrating and implementing continuous delivery pipelines.

> **Job**  
> A task or step defined in Jenkins to perform specific operations like build, test, deploy.

> **Build**  
> The process of compiling source code into binary artifacts.

> **Plugin**  
> An extension that adds new functionality to Jenkins.

> **Node**  
> Any machine (including the Master) that is part of the Jenkins environment.

> **Workspace**  
> A directory where Jenkins stores files related to a specific build.

---

## Typical Jenkins Workflow

1. **Developer pushes code** to the Version Control System (e.g., GitHub).
2. **Jenkins detects the change** using Webhooks or Polling.
3. **Jenkins triggers a build** (compiling, testing, packaging).
4. **Jenkins deploys** the application to servers or cloud environments.
5. **Reports** are generated (build success, test results).

---

## Best Practices

> **Use Pipelines as Code**  
> Prefer using `Jenkinsfile` for defining build pipelines instead of configuring them manually.

> **Secure Jenkins**  
> Always set up proper authentication and authorization.

> **Backup Regularly**  
> Backup `JENKINS_HOME` and job configurations.

> **Use Fewer Plugins**  
> Only install necessary plugins to reduce maintenance and security risks.

> **Label Agents**  
> Label nodes based on their capabilities to schedule jobs efficiently.

---

## References

- [Official Jenkins Documentation](https://www.jenkins.io/doc/)
- [Jenkins GitHub Repository](https://github.com/jenkinsci/jenkins)

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---
