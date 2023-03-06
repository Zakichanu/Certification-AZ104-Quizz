# LAB 7 of training course quizz

## Table of Contents

- [LAB 7 of training course quizz](#lab-7-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [LAB 07 (CSR): Manage Azure Storage](#lab-07-csr-manage-azure-storage)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

## LAB 07 (CSR): Manage Azure Storage

### Question 1

`You have an existing storage account in Microsoft Azure. It stores unstructured data. You create a new storage account. You need to move half of the data from the existing storage account to the new storage account. What tool should you use?
Select one:`

- Use the Azure portal
- Use File Server Resource Manager
- Use the Robocopy command-line tool
- Use the AzCopy command-line tool

<details>

    <summary>Answer</summary>

    - Use the AzCopy command-line tool

    > Why?

    Use the AzCopy command-line tool. AzCopy is a command-line utility that you can use to copy data to and from a storage account. You can use AzCopy to copy blobs, files, and tables. You can also use AzCopy to copy data between storage accounts or between a storage account and a file system.

</details>

### Question 2

```text

You are planning a delegation model for your Azure storage. The company has issued the following requirements for Azure storage access:


● Apps in the non-production environment must have automated time-limited access
● Apps in the production environment must have unrestricted access to storage resources


You need to configure storage access to meet the requirements. What should you do?
Each answer presents part of the solution. Select two:

```

- Use shared access signatures for the non-production apps.
- Use shared access signatures for the production apps.
- Use access keys for the non-production apps.
- Use access keys for the production apps.
- Use Stored Access Policies for the production apps.
- Use Cross Origin Resource Sharing for the non-production apps.


<details>

    <summary>Answer</summary>

    - Use access keys for the production apps.
    - Use shared access signatures for the non-production apps.

    > Why?

    Shared access signatures provide a way to provide more granular storage access than access keys. For example, you can limit access to “read only” and you can limit the services and types of resources. Shared access signatures can be configured for a specified amount of time, which meets the scenario’s requirements. Access keys provide unrestricted access to the storage resources, which is the requirement for production apps in this scenario.

</details>

### Question 3

`You need to provide a contingent staff employee temporary read-only access to the contents of an Azure storage account container named media. It is important that you grant access while adhering to the security principle of least-privilege. What should you do?
Select one:`

- Set the public access level to Container.
- Generate a shared access signature (SAS) token for the container.
- Share the container entity tag (Etag) with the contingent staff member.
- Configure a Cross-Origin Resource Sharing (CORS) rule for the storage account.

<details>

    <summary>Answer</summary>

    - Generate a shared access signature (SAS) token for the container.

    > Why?

    You should generate a SAS token for the container which provides access either to entire containers or blobs. You should not share the Etag with the contingent staff member. Azure uses Etags to control concurrent access to resources and do not deliver the appropriate security controls. Setting the public access level to Container would not conform to the principle of least privilege as the container now becomes open to public connections with no time limitation. CORS is a Hypertest Transfer Protocol (HTTP) mechanism that enables cross-domain resource access but does not provide security-based resource access control.

</details>

[Back to top](#table-of-contents)
