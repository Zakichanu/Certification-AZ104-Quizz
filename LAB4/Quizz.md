# LAB 4 of training course quizz

## Table of Contents

- [LAB 4 of training course quizz](#lab-4-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [Module 04A (CSR): Implement Virtual Networking](#module-04a-csr-implement-virtual-networking)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)
    - [Question 4](#question-4)
    - [Question 5](#question-5)
    - [Question 6](#question-6)
    - [Question 7](#question-7)
    - [Question 8](#question-8)
    - [Question 9](#question-9)


## Module 04A (CSR): Implement Virtual Networking

### Question 1

`Your company has an existing Azure tenant named Alpineskihouse.onmicrosoft.com. The company wants to start using alpineskihouse.com for their Azure resources. You add a custom domain to Azure. Now, you need to add a DNS record to prepare for verifying the custom domain. Which two of the following record types could you create?`

- Add an PTR record to the DNS zone.
- Add a TXT record to the DNS zone.
- Add an MX record to the DNS zone.
- Add an SRV record to the DNS zone.
- Add a CNAME record to the DNS zone.

<details>
    <summary>Answer</summary>

    - Add a TXT record to the DNS zone.
    - Add an MX record to the DNS zone.

    > Why?

    By default, Azure will prompt you to create a custom TXT record in your DNS zone to verify a custom domain. Optionally, you can use an MX record instead. The result is the same. Other record types are not supported.

</details>

### Question 2

```txt
You are planning to configure networking in Microsoft Azure. Your company has a new Microsoft Azure presence with the following network characteristics:


● 1 Virtual Network.
● 1 subnet using 192.168.0.0/23 (does not have existing resources).


Your on-premises data center has the following network characteristics:


● 10 subnets using 192.168.1.0/24 through 192.168.10.0/24.


The company intends to use 192.168.1.0/24 on-premises and 192.168.0.0/24 in Azure. You need to update your company's environment to enable the needed functionality. What should you do? Each answer represents part of the solution.
```

- Delete 192.168.0.0/23 from Azure.
- Delete 192.168.1.0/24 in the on-premises environment.
- Create a matching public subnet in Azure and in the on-premises environment.
- Create a subnet for 192.168.0.0/23 in the on-premises environment.
- Create a subnet for 192.168.0.0/24 in Azure.

<details>
    <summary>Answer</summary>

    - Delete 192.168.0.0/23 from Azure.
    - Create a subnet for 192.168.0.0/24 in Azure.

    > Why?

    Correct!
    First, you need to delete 192.168.0.0/23 from Azure. It overlaps with 192.168.1.0/24, which you intend to use for on-premises. Second, you need to create a subnet for 192.168.0.0/24 in Azure to enable usage in Azure.

</details>

### Question 3

```txt

You are planning your Azure network implementation to support your company's migration to Azure. Your first task is to prepare for the deployment of the first set of VMs. The first set of VMs that you are deploying have the following requirements:


● Consumers on the internet must be able to communicate directly with the web application on the VMs.
● The IP configuration must be zone redundant.


You need to configure the environment to prepare for the first VM. Additionally, you need to minimize costs, whenever possible, while still meeting the requirements. What should you do?
Select one:

```

- Create a standard public IP address. During the creation of the first VM, associate the public IP address with the VM's NIC.
- Create a standard public IP address. After the first VM is created, remove the private IP address and assign the public IP address to the NIC.
- Create a basic public IP address. During the creation of the first VM, associate the public IP address with the VM.
- Create a basic public IP address. After the first VM is created, remove the private IP address and assign the public IP address to the NIC.

<details>
    <summary>Answer</summary>

    - Create a standard public IP address. During the creation of the first VM, associate the public IP address with the VM's NIC.

    > Why?

    Correct!
    You need to create a standard public IP address. This is because you need to support zone redundancy. You also need to associate the public IP address with the VM's NIC during the creation of the first VM. This is because you need to support direct communication with the web application on the VMs.

</details>


### Question 4

```txt
You deploy a new domain named contoso.com to domain controllers in Azure. You have the following domain-joined VMs in Azure:


● VM1 at 10.20.30.10
● VM2 at 10.20.30.11
● VM3 at 10.20.30.12
● VM99 at 10.20.40.101


You need to add DNS records so that the hostnames resolve to their respective IP addresses. Additionally, you need to add a DNS record so that intranet.contoso.com resolves to VM99. What should you do?
(Each answer presents part of the solution. Choose two.)
```

- Add AAAA records for each VM.
- Add A records for each VM.
- Add a TXT record for intranet.contoso.com with the text of VM99.contoso.com.
- Add an SRV record for intranet.contoso.com with the target pointing at VM99.contoso.com.
- Add a CNAME record for intranet.contoso.com with a value of VM99.contoso.com.

<details>
    <summary>Answer</summary>

    - Add A records for each VM.
    - Add a CNAME record for intranet.contoso.com with a value of VM99.contoso.com.

    > Why?

    Correct!
    In this scenario, the hostnames have IPv4 IP addresses. Thus, to resolve those hostnames, you must add A records for each of the VMs. To enable intranet.contoso.com to resolve to VM99.contoso.com, you need to add a CNAME record. A CNAME record is often referred to as an “alias”.

</details>

### Question 5

```txt
Your company is preparing to move some services and VMs to Microsoft Azure. The company has opted to use Azure DNS to provide name resolution. A project begins to configure the name resolution. The project identifies the following requirements:


● A new domain will be used.
● The domain will have DNS records for internal and external resources.
● Minimize ongoing administrative overhead.


You need to prepare and configure the environment with a new domain name and a test hostname of WWW. Which of the following steps should you perform?
(Each answer presents part of the solution. Choose three.)

```

- Register a domain name with a domain registrar.
- Register a domain name with Microsoft Azure.
- Delegate the new domain name to Azure DNS.
- Add an Address (A) record for Azure name servers in the zone.
- Add DNS glue records to point to the Azure name servers.
- Add a record for WWW.

<details>
    <summary>Answer</summary>

    - Register a domain name with a domain registrar.
    - Delegate the new domain name to Azure DNS.
    - Add a record for WWW.

    > Why?

    Correct!
    For private domain names, you must register with a registrar because Azure isn't a registrar. Thereafter, you need to delegate the new domain name to Azure DNS, which enables Azure DNS to be authoritative for the domain. After delegation, you should add a test hostname of WWW and test name resolution.

</details>

### Question 6

```txt
You have a VM with two NICs named NIC1 and NIC2. NIC1 is connected to the 10.10.8.0/24 subnet. NIC2 is connected to the 10.20.8.0/24 subnet. You plan to update the VM configuration to provide the following functionality:


● Enable direct communication from the internet to TCP port 443.
● Maintain existing communication across the 10.10.8.0/24 and 10.20.8.0/24 subnets.
● Maintain a simple configuration whenever possible.


You need to update the VM configuration to support the new functionality. What should you do?
Select one:

```

- Remove the private IP address from NIC2 and then assign a public IP address to it. Then, create an inbound security rule.
- Add a third NIC and associate a public IP address to it. Then, create an inbound security rule.
- Associate a public IP address to NIC2 and create an inbound security rule.
- Create an inbound security rule for TCP port 443.

<details>
    <summary>Answer</summary>

    - Associate a public IP address to NIC2 and create an inbound security rule.

    > Why?

    Correct!
    To enable direct communication from the internet to the VM, you must have a public IP address. You also need an inbound security rule. You can associate the public IP address with NIC1 or NIC2, although this scenario only presents an option to associate it with NIC2 so that is the correct answer.

</details>

### Question 7

```txt

You're currently using network security groups (NSGs) to control how your network traffic flows in and out of your virtual network subnets and network interfaces. You want to customize how your NSGs work. For all incoming traffic, you need to apply your security rules to both the virtual machine and subnet level.
Which of the following options will let you accomplish this? (Choose two)

```

- Configure the AllowVNetInBound security rule for all new NSGs.
- Create rules for both NICs and subnets with an allow action.
- Delete the default rules.
- Add rules with a higher priority than the default rules.

<details>
    <summary>Answer</summary>

    - Create rules for both NICs and subnets with an allow action.
    - Add rules with a higher priority than the default rules.

    > Why?

    Correct!
    You can create rules for both NICs and subnets with an allow action. You can also add rules with a higher priority than the default rules. This will allow you to customize how your NSGs work.

</details>

### Question 8

```txt
You need to ensure that Azure DNS can resolve names for your registered domain. What should you implement?
Select one:

```

- zone delegation
- a CNAME record
- an MX record
- a secondary zone
- a primary zone with a NS record

<details>
    <summary>Answer</summary>

    - zone delegation

    > Why?

    Correct!
    To ensure that Azure DNS can resolve names for your registered domain, you need to implement zone delegation. This is because Azure DNS is not a registrar. You must register your domain with a registrar and then delegate the domain to Azure DNS.

</details>

### Question 9

```txt

You are configuring the Azure Firewall. You need to allow Windows Update network traffic through the firewall. Which of the following should you use?
Select one:

```

- Application rules
- Destination inbound rules
- NAT rules
- Network rules

<details>
    <summary>Answer</summary>

    - Application rules

    > Why?

    Correct!
    Application rules are used to allow or deny traffic based on the application layer. In this scenario, you need to allow Windows Update network traffic through the firewall. This is an application layer rule.

</details>

[Back to Top](#table-of-contents)