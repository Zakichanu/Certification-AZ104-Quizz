# LAB 2 of training course quizz

## Table of Contents

- [LAB 2 of training course quizz](#lab-2-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [Lab 02A (Manage Subscriptions and RBAC) \& Lab 02B (Manage Governance and Compliance) Review Questions](#lab-02a-manage-subscriptions-and-rbac--lab-02b-manage-governance-and-compliance-review-questions)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

## Lab 02A (Manage Subscriptions and RBAC) & Lab 02B (Manage Governance and Compliance) Review Questions

### Question 1

`You need to target policies and review spend budgets across several subscriptions you manage. What should you do?
Select one:`

- Create resource groups
- Create management groups
- Create billing groups
- Create Azure policies

<details>
    <summary>Answer</summary>

    Create management groups

    > Why?

    Management groups are a way to organize your subscriptions. You can create management groups to organize your
    subscriptions and apply policies to enforce governance across your subscriptions. You can also create management groups
    to apply budgets to monitor your spend across your subscriptions.
</details>

### Question 2

`You would like to categorize resources and billing for different departments like IT and HR. The billing needs to be consolidated across multiple resource groups and you need to ensure everyone complies with the solution. What should you do?
{Choose two to complete a solution}:`

- Create tags for each department.
- Create a billing group for each department.
- Create an Azure policy.
- Add the groups into a single resource group.
- Create a subscription account rule.

<details>
    <summary>Answer</summary>

    - Create tags for each department.
    - Create an Azure policy.

    > Why?

    Create tags for each department and Create an Azure policy. You should create a tag with a key:value pair like
    department:HR. You can then create an Azure policy which requires the tag be applied before a resource is created.
</details>

### Question 3

`Your company financial comptroller wants to be notified whenever the company is half-way to spending the money allocated for cloud services. What should you do?
Select one:`

- Create an Azure reservation.
- Create a budget and a spending threshold.
- Create a management group.
- Enter workloads in the Total Cost of Ownership calculator.

<details>
    <summary>Answer</summary>

    Create a budget and a spending threshold.

    > Why?

    Create a budget and a spending threshold. Billing Alerts help you monitor and manage billing activity for your Azure
    accounts. You can set up a total of five billing alerts per subscription, with a different threshold and up to two email
    recipients for each alert. Monthly budgets are evaluated against spending every four hours. Budgets reset automatically
    at the end of a period.
</details>

[Back to Top](#table-of-contents)