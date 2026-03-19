# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : Gokul Nath R
Reg no : 212224230077
Date : 19-03-2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. Logged into the AWS Management Console and reviewed the existing EC2 architecture created in previous labs.
2. Created a Launch Template by selecting an AMI, instance type, key pair, security group, and added user data for application setup.
3. Configured an Auto Scaling Group (ASG) using the launch template and set minimum, desired, and maximum number of instances.
4. Created an Application Load Balancer (ALB) and configured listeners and a target group.
5. Attached the Auto Scaling Group to the target group so that traffic is distributed across instances.
6. Set up scaling policies using CloudWatch alarms based on CPU utilization (scale out and scale in conditions).
7. Generated traffic to test the system and observed automatic scaling and load balancing across EC2 instances.
8. Verified fault tolerance by stopping an instance and confirming that the ASG launched a new instance automatically.


---

## Output Screenshots 

<img width="1919" height="1038" alt="Screenshot 2026-03-19 134946" src="https://github.com/user-attachments/assets/a40b9b59-0c45-4b66-8710-9289c1d8190e" />
<img width="1919" height="1043" alt="Screenshot 2026-03-19 135256" src="https://github.com/user-attachments/assets/6c425d7f-c2f9-4984-ac14-a6033835e46c" />
<img width="1919" height="1041" alt="Screenshot 2026-03-19 135622" src="https://github.com/user-attachments/assets/a4971439-5622-41d0-9b16-b6a8009f8bcd" />
<img width="1918" height="1047" alt="Screenshot 2026-03-19 144347" src="https://github.com/user-attachments/assets/f847fc93-35f1-4104-999c-10a3b068659f" />
<img width="1915" height="1047" alt="Screenshot 2026-03-19 144720" src="https://github.com/user-attachments/assets/35f90f68-85f2-44f5-ae12-b4c554aae544" />
<img width="1919" height="1087" alt="Screenshot 2026-03-19 145732" src="https://github.com/user-attachments/assets/ed09adc5-e3dd-4808-bd08-adda77ccb27a" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
