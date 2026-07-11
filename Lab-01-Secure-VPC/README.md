# Lab 01 - Secure AWS VPC

## Objective

Design and build a secure Virtual Private Cloud (VPC) in AWS that follows best practices for networking and security
---

## Business Scenario

A company wants to move one of its web applications from an on-premises data center to AWS.

The APPLICATION MUST:

- Be secure
- Be scalable
- Allow customers to access the website
- Keep the database private
- Follow AWS networking best practices

---

## AWS Services Used

- Amazon VPC
- Public Subnets
- Private Subnets
- Internet Gateway
- Route Tables
- Security Groups
- Network ACLs

---

## Architecture Diagram

(To be added after completing the lab.)

---

## VPC Created

![VPC Created](..Images/Lab01-01-VPC-Created.png)

## Public Route Table

![Public Route Table](..Images/Lab01-02-Public-Route-Table.png)

## Web Server Security Group

![Web Server Security Group](..Images/Lab01-03-WebServer-SecurityGroup.png)

---

## Lessons Learned

During this lab I learned how to design and build a secure Virtual Private Cloud (VPC) in AWS.

Key concepts learned:

- Created a custom VPC using the 10.0.0.0/16 CIDER block.
- Designed a highly available network across two Availability Zones.
- Configured public and private subnets.
- Learned that a subnet is public because its route table contains a default route (0.0.0.0/0) To an Internet Gateway.
- Learned that private subnets do not have a direct route to an Internet Gateway.
- Created a custom Security Group for a web server.
- Configured HTTP, HTTPS, and SSH access using security best practices.
- Learned the importance of restricting SSH access to trusted IP addresses.