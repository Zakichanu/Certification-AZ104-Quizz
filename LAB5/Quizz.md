# LAB 5 of training course quizz

## Table of Contents

- [LAB 5 of training course quizz](#lab-5-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [LAB 05 (CSR): Implement Intersite Connectivity](#lab-05-csr-implement-intersite-connectivity)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)


## LAB 05 (CSR): Implement Intersite Connectivity

### Question 1

`You want to connect different VNets in the same region as well as different regions and decide to use VNet peering to accomplish this. Which of the following statements is not true about VNet peering?
Select one:`

- The virtual networks can only exist in the same azure cloud region.
- Network traffic between peered virtual networks is private.
- Peering is easy to configure and manage, requiring little to no downtime.
- Gateway transit can be configured regionally or globally.

<details>
    <summary>Answer</summary>

    The virtual networks can only exist in the same azure cloud region.

    > Why?

    The virtual networks can exist in any Azure cloud region.
</details>

### Question 2

```

    Your company is preparing to implement a Site-to-Site VPN to Microsoft Azure. You are selected to plan and implement 
    the VPN. Currently, you have an Azure subscription, an Azure virtual network, and an Azure gateway subnet. You need to 
    prepare the on-premises environment and Microsoft Azure to meet the prerequisites of the Site-to-Site VPN. Later, you 
    will create the VPN connection and test it. What should you do?

    Each answer presents part of the solution. 
    Select three.
```

- Obtain a VPN device for the on-premises environment.
- Obtain a VPN device for the Azure environment.
- Create a virtual network gateway (VPN) and the local network gateway in Azure.
- Create a virtual network gateway (ExpressRoute) in Azure.
- Obtain a public IPv4 IP address without NAT for the VPN device.
- Obtain a public IPv4 IP address behind NAT for the VPN device.

<details>
    <summary>Answer</summary>

    - Obtain a VPN device for the on-premises environment.
    - Create a virtual network gateway (VPN) and the local network gateway in Azure.
    - Obtain a public IPv4 IP address without NAT for the VPN device.

    > Why?

    The prerequisites for a Site-to-Site VPN are having a compatible VPN device on-premises, having a public IPv4 IP without NAT on the on-premises VPN device, and creating a VPN gateway and local network gateway in Azure. IPv6 is not supported for VPNs. ExpressRoute is a different setup and not part of a Site-to-Site VPN.

</details>

### Question 3

```
    Your company is preparing to implement persistent connectivity to Microsoft Azure. The company has a single site, headquarters, which has an on-premises data center. The company establishes the following requirements for the connectivity:


● Connectivity must be persistent.
● Connectivity must provide for the entire on-premises site.


You need to implement a connectivity solution to meet the requirements. What should you do?
Select one:*
```

- Implement a Site-to-Site VPN.
- Implement a Virtual Private Cloud (VPC).
- Implement a Virtual Private Gateway (VGW).
- Implement a VNet-to-VNet VPN.
- Implement a Point-to-Site VPN.

<details>
    <summary>Answer</summary>

    Implement a Site-to-Site VPN.

    > Why?

    In this scenario, only one of the answers provides persistent connectivity to Azure - the Site-to-Site VPN. A VNet-to-VNet connects two Azure virtual networks together. A Point-to-Site VPN is used for individual connections (such as for a developer). A VPC and VGW are relevant to Amazon AWS.

</details>


[Back to Top](#table-of-contents)