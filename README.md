# Databricks Declarative Automation Bundles (DAB) Tutorial

##  Overview

This repository demonstrates how to use **Declarative Automation Bundles (DAB)** in Databricks to manage data engineering projects using modern software engineering practices.

DAB helps in packaging code, configuration, and infrastructure into a single deployable unit, enabling automation, scalability, and collaboration.

---

##  Objectives

* Understand **Databricks CLI**
* Learn **Declarative Automation Bundles (DAB)**
* Implement **bundle lifecycle (init → validate → deploy)**
* Integrate with **Git & CI/CD workflows**

---

##  What is DAB?

Declarative Automation Bundles allow you to:

* Define Databricks resources (jobs, pipelines) as code
* Use **YAML configuration (databricks.yml)**
* Automate deployment using CLI
* Follow best practices like:

  * Source control
  * Code review
  * Testing
  * CI/CD

---

##  Project Structure

```
dabtutorial/
│── databricks.yml        # Main configuration file
│── resources/            # Job / pipeline definitions
│── src/                  # Source code (ETL / Python)
│── README.md             # Project documentation
```

---

##  Prerequisites

Before running this project, ensure you have:

* Databricks account
* Databricks CLI (v0.218.0 or above)
* Git installed
* Access to Databricks workspace

---

##  Setup & Authentication

Login using Databricks CLI:

```
databricks auth login
```

Check profiles:

```
databricks auth profiles
```

---

## Getting Started

### 1️. Initialize Bundle

```
databricks bundle init
```

---

### 2️. Validate Bundle

```
databricks bundle validate
```

---

### 3️. Deploy Bundle

```
databricks bundle deploy --target dev
```

---

### 4️. Run Workflows

```
databricks bundle run
```

---

##  Bundle Lifecycle

1. Initialize bundle
2. Develop (code + YAML config)
3. Validate
4. Deploy
5. Execute workflows

---

##  Key Components

* **databricks.yml** → Main configuration
* **resources/** → Jobs & pipelines
* **src/** → Business logic
* **targets (dev/prod)** → Environment configuration

---

##  CI/CD Workflow

* Develop locally
* Push code to GitHub
* Trigger CI/CD pipeline
* Deploy to:

  * Dev
  * Staging
  * Production

---

##  Benefits of DAB

* Standardized project structure
* Automated deployments
* Easy collaboration
* Infrastructure as Code (IaC)
* Reduced manual effort


## Author

**Payal Pravin Sarode**

---

##  Notes

This project is created for learning and demonstration purposes to understand how DAB simplifies Databricks workflows.

---

##  Future Enhancements

* Add CI/CD pipeline integration
* Add real ETL pipeline
* Add ML workflow example

---
