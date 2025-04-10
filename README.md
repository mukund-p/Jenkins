# Jenkins_Basics

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

![Jenkins Logo](https://www.jenkins.io/images/logos/jenkins/jenkins.png)

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

![Jenkins Architecture](https://miro.medium.com/max/1400/1*TL5hGsFZkt9nJmw-H9DNMg.png)

> **Master (Controller)**  
> - Orchestrates the tasks  
> - Schedules jobs, manages agents, monitors builds  

> **Agent (Node/Slave)**  
> - Executes the tasks assigned by the master  
> - Helps in load balancing

---

## Basic Jenkins Terminology

> **Job / Project**  
> A task like building, testing, or deploying software.

> **Build**  
> A single run of a project.

> **Pipeline**  
> A suite of plugins that supports integrating and implementing continuous delivery pipelines.

> **Executor**  
> A computational slot on an agent where a job runs.

> **Plugin**  
> A module that extends Jenkins' capabilities.

---

## Typical Jenkins Workflow

```plaintext
1. Developer pushes code to Version Control (e.g., GitHub).
2. Jenkins detects code changes (via webhook or polling).
3. Jenkins pulls the latest code.
4. Jenkins builds the application.
5. Jenkins runs tests.
6. Jenkins deploys the build to the server (if successful).
7. Jenkins notifies the team (via email, Slack, etc.).
