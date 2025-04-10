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
It helps implement Continuous Integration and Continuous Delivery (CI/CD) in a project.

---

## Key Features of Jenkins
> **Open Source**:  
> Free to use with a large community.

> **Extensible**:  
> Supports over 1,800+ plugins for building, deploying, and automating.

> **Distributed Builds**:  
> Supports Master-Agent architecture to manage multiple builds.

> **Easy Installation**:  
> Simple to install via `.war` file, Docker, or package manager.

> **Rich UI and APIs**:  
> Provides a user-friendly web interface and REST APIs.

---

## Jenkins Architecture
> **Master (Controller)**:  
> Coordinates the tasks, schedules builds, and manages agents.

> **Agent (Node/Slave)**:  
> Machines that perform the actual build tasks as instructed by the master.

> **Executor**:  
> A slot for a job to run on an agent.

---

## Basic Jenkins Terminology

> **Job / Project**:  
> A task like building code, running tests, or deploying.

> **Build**:  
> The actual running instance of a job.

> **Pipeline**:  
> A suite of steps to automate the software delivery process.

> **Plugin**:  
> An extension that adds functionality to Jenkins.

> **Workspace**:  
> Directory where Jenkins keeps files related to a job.

---

## Typical Jenkins Workflow
1. **Developer pushes code** to a Version Control System (e.g., GitHub).
2. **Jenkins detects changes** (polling or webhook).
3. **Jenkins pulls the code** and performs the build.
4. **Tests are executed** automatically.
5. **Build artifacts** are generated and stored.
6. **Deployment is triggered** to staging or production.

---

## Best Practices
> **Use Pipelines**:  
> Prefer Pipeline-as-Code (`Jenkinsfile`) over freestyle jobs for better version control.

> **Secure Jenkins**:  
> Always configure user authentication, authorization, and install security plugins.

> **Keep Jenkins Updated**:  
> Regularly update Jenkins and plugins to get security patches and new features.

> **Use Agents Efficiently**:  
> Offload heavy build jobs to agents instead of running on the master.

> **Monitor Jenkins Health**:  
> Regularly backup your Jenkins server and monitor system performance.

---

> 📄 This document is maintained by Mukund Patil.
