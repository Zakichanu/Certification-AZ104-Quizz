# LAB 8 of training course quizz

## Table of Contents

- [LAB 8 of training course quizz](#lab-8-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [Module 08 (CSS): Manage Virtual Machines](#module-08-css-manage-virtual-machines)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

## Module 08 (CSS): Manage Virtual Machines

### Question 1

`You host a service with two Azure virtual machines. You discover that occasional outages cause your service to fail. What two actions can you do to minimize the impact of the outages?
Select two:`

- Add a load balancer.
- Put the virtual machines in an availability set.
- Put the virtual machines in a scale set.
- Add a network gateway.
- Add a third instance of the virtual machine.

<details>
    <summary>Answer</summary>

    - Put the virtual machines in an availability set.
    - Add a load balancer.

    > Why?

    To minimize the impact put the virtual machines in an availability set and add a load balancer

</details>

### Question 2

`Another IT administrator creates an Azure virtual machine scale set with 5 VMs. Later, you notice that the VMs are all running at max capacity with the CPU being fully consumed. However, additional VMs are not deploying in the scale set. You need to ensure that additional VMs are deployed when the CPU is 75% consumed. What should you do?
Select one:`

- Enable the autoscale option.
- Increase the instance count.
- Add the scale set automation script to the library.
- Deploy the scale set automation script.

<details>
    <summary>Answer</summary>

    - Enable the autoscale option.

    > Why?

    When you have a scale set, you can enable automatic scaling with the autoscale option. When you enable the option, you define the parameters for when to scale. To meet the requirements of this scenario, you need to enable the autoscale option so that additional VMs are created when the CPU is 75% consumed. Note that the automation script is used to automate the deployment of scale sets and not related to automating the building of additional VMs in the scale set.

</details>

### Question 3

`Your organization has a security policy that prohibits exposing SSH ports to the outside world. You need to connect to an Azure Linux virtual machine to install software. What should you do?
Select one:`

- Configure the Bastion service
- Configure a Guest configuration on the virtual machine
- Create a custom script extension
- Work offline and then reimage the virtual machine.

<details>
    <summary>Answer</summary>

    - Configure the Bastion service

    > Why?

    Configure the Bastion service. The Azure Bastion service is a new fully platform-managed PaaS service that you provision inside your virtual network. It provides secure and seamless RDP and SSH connectivity to your virtual machines directly in the Azure portal over SSL. When you connect via Azure Bastion, your virtual machines do not need a public IP address.

    Bastion provides secure RDP and SSH connectivity to all VMs in the virtual network in which it is provisioned. Using Azure Bastion protects your virtual machines from exposing RDP and SSH ports to the outside world while still providing secure access using RDP and SSH. With Azure Bastion, you connect to the virtual machine directly from the Azure portal. You don't need an additional client, agent, or piece of software

</details>

[Back to top](#table-of-contents)