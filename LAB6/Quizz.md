# LAB 6 of training course quizz

## Table of Contents

- [LAB 6 of training course quizz](#lab-6-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [LAB 06 (CSS): Implement Traffic Management](#lab-06-css-implement-traffic-management)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

## LAB 06 (CSS): Implement Traffic Management

### Question 1

`Which of the following two features of Azure networking provide the ability to redirect all Internet traffic back to your company's on-premises servers for packet inspection?
Select two:`

- User Defined Routes
- Cross-premises network connectivity
- Traffic Manager
- Forced Tunneling
- System Routes

<details>
    <summary>Answer</summary>

    - Forced Tunneling
    - User Defined Routes

    > Why?

    User defined routes and forced tunneling. You can use forced tunneling to redirect internet bound traffic back to the company's on-premises infrastructure. Forced tunneling is commonly used in scenarios where organizations want to implement packet inspection or corporate audits. Forced tunneling in Azure is configured via virtual network user defined routes (UDR).
</details>

### Question 2

`Your company provides customers a virtual network in the cloud. You have dozens of Linux virtual machines in another virtual network. You need to install an Azure load balancer to direct traffic between the virtual networks. What should you do?
Select one:`

- Install a private load balancer.
- Install a public load balancer.
- Install an external load balancer.
- Install an internal load balancer.
- Install a network load balancer.

<details>
    <summary>Answer</summary>

    - Install an internal load balancer.

    > Why?

    Install an internal load balancer. Azure has two types of load balancers: public and internal. An internal load balancer directs traffic only to resources that are inside a virtual network or that use a VPN to access Azure infrastructure.

</details>

### Question 3

`You have a virtual network with a subnet that contains a virtual machine. You need to configure the virtual machine to use a static private IP address. What should you do?`

- Install an external load balancer
- Install an internal load balancer
- Install Azure Firewall
- Install the Web Application Firewall

<details>
    <summary>Answer</summary>

    - Install the Web Application Firewall

    > Why?

    Install the Web Application Firewall. The web application firewall (WAF) is an optional component that handles incoming requests before they reach a listener. The web application firewall checks each request for many common threats, based on the Open Web Application Security Project (OWASP).
</details>

[Back to top](#table-of-contents)