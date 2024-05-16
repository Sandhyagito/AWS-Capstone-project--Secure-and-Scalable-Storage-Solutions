# AWS-Capstone-project--Secure-and-Scalable-Storage-Solutions

Spearheaded the design and implementation of a robust AWS Elastic File System (EFS) to provide a highly available, secure, and persistent storage solution. The initiative focused on creating a reliable data storage system that ensures seamless accessibility across multiple servers.

**Problem Statement:**
ABC is India based entertainment production company with a focus on Northeast and East Indian cinema. They wanted a highly available and reliable storage solution for their on-prem data. The client wanted the data to be reliable, highly available, secure, and persistent, and also wanted to have data on the storage to be accessible from all the servers. The issues with the existing infrastructure are mentioned below: 

 1) They were using NAS storage which had limitations in scalability.

 2) The client wanted a complete application to run in Aws cloud with storage in the 
 cloud to keep his files in sync with servers so that he has centralized storage of data 

 3) There were security issues in the existing infrastructure and no encryption at rest or 
 Transit.

 4) Manual intervention was needed to change the storage type and transfer files to 
 infrequent storage. 

 5) The client is unable to scale up the infrastructure due to high capital costs for new 
 hardware. 

 6) Need for low-cost storage options for both frequent and infrequent data.

 7) Highly available, secure, and persistent shared File system in AWS cloud with EFS

**Components**:

**EFS** - Amazon EFS (Elastic File System) provides a simple, scalable, fully managed elastic NFS file system.
Can serve as a centralized storage solution that is accessible from all servers, keeping files in sync across the entire infrastructure.

**KMS** - AWS Key Management Service (KMS) is a secure service that helps you manage and control encryption keys.

**EC2** - Amazon EC2 (Elastic Compute Cloud) offers scalable computing capacity in the AWS cloud, which allows ABC to increase or decrease capacity. This addresses the scalability limitations of their current NAS storage

**Solution**

**Challenge Overview:** ABC found itself constrained by a legacy NAS storage system, which lacked the necessary scalability and posed significant security vulnerabilities. The company’s vision to migrate to a cloud-based application with centralized data synchronization was hindered by the existing infrastructure’s limitations.

**Strategic Solution:**
We created a **highly available, reliable, and secure storage distributed file system** using Amazon Elastic File System (EFS), which **allows multiple EC2 instances to share data efficiently and securely**.

**Security and Reliability:** 
To safeguard our data, we integrated **AWS Key Management Service (KMS)**, ensuring **all data stored in EFS is encrypted** and protected against unauthorized access. Also, We tackled the pressing concerns of data encryption both at rest and in transit implementing KMS fortify data integrity and confidentiality

**Infrastructure Setup:** 
Our setup included configuring EC2 instances with **custom security groups within a VPC designed for EFS**, enabling secure communication and data transfer.

**Cost-Effective Scaling:** By leveraging AWS’s cloud infrastructure, we eliminated the need for costly hardware investments, **enabling ABC to dynamically scale their storage capabilities while optimizing costs for both frequently and infrequently accessed data**

**Resilience and Redundancy:** 
We demonstrated resilience by launching EC2 instances across **different availability zones**, ensuring our system remains robust against potential zone failures.

**Hands-On Execution:** 
The practical aspect involved connecting to EC2 instances, installing necessary utilities, and mounting the EFS filesystem to validate real-time data sharing and synchronization

![diagram-export-5-4-2024-9_58_01-PM](https://github.com/Sandhyagito/AWS-Capstone-project--Secure-and-Scalable-Storage-Solutions/assets/151674108/ca615c96-bdbf-483f-ba41-f89c5051b028)
