# Lab 9 of training course quizz

## Table of Contents

- [Lab 9 of training course quizz](#lab-9-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [LAB 09A (CSR): Implement Web Apps](#lab-09a-csr-implement-web-apps)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)
  - [LAB 09B (CSS): Implement Containers](#lab-09b-css-implement-containers)
    - [Question 1](#question-1-1)
    - [Question 2](#question-2-1)
    - [Question 3](#question-3-1)
  - [LAB 09C (CSS): Implement Azure Kubernetes Service](#lab-09c-css-implement-azure-kubernetes-service)
    - [Question 1](#question-1-2)
    - [Question 2](#question-2-2)
    - [Question 3](#question-3-2)

## LAB 09A (CSR): Implement Web Apps

### Question 1

`You have multiple apps running in a single App Service plan. True or False: Each app in the service plan can have different scaling rules.`

- True
- False

<details>
    <summary>Answer</summary>

    - False

    > Why?

    False. The App Service plan is the scale unit of the App Service apps. If the plan is configured to run five VM instances, then all apps in the plan run on all five instances. If the plan is configured for autoscaling, then all apps in the plan are scaled out together based on the autoscale settings.

</details>

### Question 2

`Which of the following settings are not not swapped when you swap an an app?
Select three:`

- Handler mappings
- Publishing endpoints
- General settings, such as framework version, 32/64-bit, web sockets
- Always On
- Custom domain names

<details>
    <summary>Answer</summary>

    - Always On
    - Publishing endpoints
    - Custom domain names

    > Why?

    Publishing endpoints, Always on, and Custom domain names. Some configuration elements follow the content across a swap (not slot specific), whereas other configuration elements stay in the same slot after a swap (slot specific).

</details>

### Question 3

`You are administering a production web app. The app requires scaling to five instances, 40GB of storage, and a custom domain name. Which App Service Plan should you select?
Select one`

- Free
- Shared
- Basic
- Standard
- Premium

<details>
    <summary>Answer</summary>

    - Standard

    > Why?

    Standard. The Standard App Service Plan meets the requirements at the least cost.

</details>

## LAB 09B (CSS): Implement Containers

### Question 1

`You have a web app that uses a custom Docker image. You need to ensure that the app is always running. Which configuration should you use?`

- App configuration
- Azure database for MySQL
- Files and database content totalling 15GB
- Firewall enabled-storage account
- SSL enabled Azure Database for MySQL

<details>
    <summary>Answer</summary>

    - App configuration
    - Azure database for MySQL

    > Why?

    App configuration and Azure database for MySQL. App Service can back up: app configuration, file content, and a database connected to your app (SQL Database, Azure Database for MySQL, Azure Database for PostgreSQL, MySQL in-app). Backups can be up to 10 GB of app and database content. Using a firewall enabled storage account as the destination for your backups is not supported. SSL enabled Azure Database for MySQL does not get backed up.

</details>

### Question 2

`You decide to move all your services to Azure Kubernetes service. Which of the following components will contribute to your monthly Azure charge?
Select one:`

- Azure managed node
- Pods
- Customer node virtual machines
- Tables

<details>
    <summary>Answer</summary>

    - Customer node virtual machines

    > Why?

    Customer node virtual machines. You only pay for the virtual machines instances, storage, and networking resources consumed by your Kubernetes cluster.

</details>

### Question 3

`Which of the following is not true about container groups?
Select one:`

- Is scheduled on a multiple host machines.
- Is assigned a DNS name label.
- Exposes a single public IP address, with one exposed port.
- Consists of two containers.
- Includes two Azure file shares as volume mounts.

<details>
    <summary>Answer</summary>

    - Is scheduled on a multiple host machines.

    > Why?

    Is scheduled on a single host machine. A container group is a logical grouping of containers that are scheduled on a single host machine. A container group is assigned a DNS name label and exposes a single public IP address, with one exposed port. A container group consists of one or more containers, and includes one or more Azure file shares as volume mounts.

</details>

## LAB 09C (CSS): Implement Azure Kubernetes Service

### Question 1

`Which of the following is the Kubernetes agent that processes the orchestration requests and schedules running the requested containers?
Select one:`

- controller
- container runtime
- kube-proxy
- kubelet

<details>
    <summary>Answer</summary>

    - kubelet

    > Why?

    kubelet. The kubelet process the orchestration requests and schedules running the requested containers

</details>

### Question 2

`You are configuring networking for the Azure Kubernetes service. Which of the following maps incoming direct traffic to the pods?
Select one:`

- AKS node
- ClusterIP
- Load Balancer
- NodePort

<details>
    <summary>Answer</summary>

    - NodePort

    > Why?

    NodePort. NodePort maps incoming direct traffic to the pods.

</details>

### Question 3

`What method does Microsoft Azure App Service use to obtain credentials for users attempting to access an app?
Select one:`

- Credentials that are stored in the browser.
- Pass-through authentication.
- Redirection to a provider endpoint.
- Synchronization of accounts across providers.

<details>
    <summary>Answer</summary>

    - Redirection to a provider endpoint.

    > Why?

    Redirection to a provider endpoint. Microsoft Azure App Service apps redirect requests to an endpoint that signs in users for that provider. The App Service can automatically direct all unauthenticated users to the endpoint that signs in users. Course: Module 4

</details>

[Back to top](#table-of-contents)