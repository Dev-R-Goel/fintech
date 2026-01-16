# FinTech Lab – REST API & Cloud Deployment

## Student: Dev Goel

## Course: FinTech Laboratory

---

## 📌 Overview

This repository contains all the work completed as part of **FinTech Lab – Experiments 1 & 2**. The lab focuses on setting up the development environment, building a **Spring Boot REST API**, version controlling the project using **Git & GitHub**, and deploying the application to **Microsoft Azure Cloud**.

---

## 🛠️ Software & Tools Used

* Java (JDK 11 / 17)
* Spring Boot
* Maven
* Eclipse IDE
* Visual Studio Code
* Node.js & npm
* Angular CLI
* MySQL
* Postman
* Git & GitHub
* Azure Cloud Shell

---

## 🔍 Installation Verification Commands

```bash
node -v
npm -v
nvm --version
ng version
code --version
mysql --version
git --version
```

---

## 🌐 REST API Concepts

A **REST API (Representational State Transfer – Application Programming Interface)** allows communication between client and server using HTTP methods.

### Key Features:

* Resource-based URLs
* Stateless communication
* CRUD operations using HTTP methods
* Data exchange using JSON

### Common HTTP Methods:

* GET – Retrieve data
* POST – Create data
* PUT – Update data
* DELETE – Remove data

---

## ⚙️ Spring Boot Project Setup

### Step 1: Spring Initializr

* Visit: https://start.spring.io/
* Project: Maven
* Language: Java
* Spring Boot: Latest stable version
* Packaging: JAR
* Java Version: 17
* Dependency: Spring Web

### Step 2: Import Project

* Open Eclipse
* File → Import → Existing Maven Project
* Select downloaded project folder

---

## ▶️ Running the Application

* Run the project using the Green Run button in Eclipse
* Access the app at:

```
http://localhost:8080/
```

If a **Whitelabel Error Page** appears, the server has started successfully.

---

## 🧩 REST Controller Implementation

```java
package com.example.demo;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class Hello {
    @GetMapping("/")
    public String index() {
        return "Greetings from MIT-FIS!";
    }
}
```

### Annotations Used:

* `@SpringBootApplication` – Main entry point
* `@RestController` – Defines REST controller
* `@GetMapping` – Maps HTTP GET requests

---

## 🗃️ Git & GitHub Version Control

### Initialize Git Repository

```bash
git init
```

### Add & Commit Files

```bash
git add .
git commit -m "Initial FinTech Lab commit"
```

### Push to GitHub

```bash
git remote add origin <repository-url>
git branch -M main
git push origin main
```

---

## ☁️ Azure Cloud Deployment

### Clone Repository in Azure Shell

```bash
git clone <repository-url>
cd my-webapp
```

### Configure Azure Web App

```bash
mvn com.microsoft.azure:azure-webapp-maven-plugin:2.13.0:config
```

Configuration Choices:

* OS: Linux
* Java Version: 17
* Region: Central India
* Pricing Tier: F1 / P1v2

### Deploy Application

```bash
mvn clean package
mvn azure-webapp:deploy
```

---

## ✅ Outcome

* Successfully built a Spring Boot REST API
* Version-controlled the project using GitHub
* Deployed the application on Azure Cloud
* Understood REST principles and cloud deployment workflow

---


## 🔚 Conclusion

This lab provided hands-on experience in full-stack backend development, REST API creation, Git-based collaboration, and cloud deployment using Azure, aligning with real-world FinTech application development practices.
