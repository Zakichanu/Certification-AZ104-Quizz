# Lab 10 of training course quizz

## Table of Contents

- [Lab 10 of training course quizz](#lab-10-of-training-course-quizz)
  - [Table of Contents](#table-of-contents)
  - [Module 10 (CSR): Backup virtual machines](#module-10-csr-backup-virtual-machines)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)

## Module 10 (CSR): Backup virtual machines

### Question 1

`Your organization needs a way to create application aware snapshots, and backup Linux virtual machines and VMware virtual machines. You have files, folders, volumes and workloads to protect. You recommend which of the following solutions?
Select one:`

- Azure Backup (MARS) agent
- Azure Backup Server
- Enable disk snapshots
- Enable backup for individual Azure VMs

<details>
    <summary>Answer</summary>

    - Azure Backup Server

    > Why?

    Azure backup server provides app aware snapshots, support for Linux virtual machines and VMware virtual machines. Backup server can protect files, folders, volumes, and workloads.

</details>

### Question 2

`You have several Azure VMs that are currently running production workloads. You have a mix of Windows Server and Linux servers and you need to implement a backup strategy for your production workloads. Which feature should you use in this case?
Select one:`

- Managed snapshots.
- Azure Backup.
- Azure Site Recovery.
- Azure Migrate.

<details>
    <summary>Answer</summary>

    - Azure Backup

    > Why?

    For backing up Azure virtual machines running production workloads, use Azure Backup. Azure Backup supports application-consistent backups for both Windows and Linux virtual machines. Azure Site Recovery coordinates virtual-machine and physical-server replication, failover, and failback, but Azure Backup will protect and restore data at a more granular level. Managed snapshots provide a read-only full copy of a managed disk, and is an ideal solution in development and test environments, but Azure Backup is the better option for your production workloads.

</details>

### Question 3

`You plan to use virtual machine soft delete. Which of the following statements are true?
Select two:`

- Soft delete provides 20 days extended retention of data.
- If you delete a backup, soft delete still provides recovery of data.
- Soft delete is built-in protection at no additional cost.
- Soft delete items are stored in archive storage.
- A recovery service vault can be deleted if it only has soft-deleted backup items.

<details>
    <summary>Answer</summary>

    - Soft delete is built-in protection at no additional cost.
    - If you delete a backup, soft delete still provides recovery of data.
    > Why?

    If you delete a backup, soft delete still provides recovery of data. Soft delete is built-in protection at no additional cost.

</details>

[Back to up]((#table-of-contents))
