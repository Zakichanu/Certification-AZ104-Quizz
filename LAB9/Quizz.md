# Lab 9 of training course quizz

## Table of Contents

- [Lab 9 of training course quizz](#lab-9-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [LAB 09A (CSR): Implement Web Apps](#lab-09a-csr-implement-web-apps)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

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

[Back to top](#table-of-contents)