

Challenge #1
=============
A 3 tier environment is a common setup. Use a tool of your choosing/familiarity create these resources.

Approach ::
=============
A three-tier architecture is a software architecture pattern where the application is broken down into three logical tiers: the presentation layer, 
the business logic layer and the data storage layer. This architecture is used in a client-server application such as a web application that has 
the frontend, the backend and the database. Each of these layers or tiers does a specific task and can be managed independently of each other. 
This is a shift from the monolithic way of building an application where the frontend, the backend and the database are both sitting in one place.

Amazon Web Service (AWS) is a cloud platform that provides different cloud computing services to their customers.To demonstrate, we shall 
be making use of the following AWS services to design and build a three-tier cloud infrastructure: Elastic Compute Cloud (EC2), Auto Scaling Group, 
Virtual Private Cloud(VPC), Elastic Load Balancer (ELB), Security Groups and the Internet Gateway. Our infrastructure will be designed to be 
highly available and fault tolerant.

Options 
=============
To follow along, we need to have an AWS account and will create below all services through AWS Console. 
This can be achieved through Terraform IAC automation as well so that same can be easily available for other client and workgroup.

What we need?
===============

    1. VPC
    2. Internet gateway
    3. 4 Subnets (2 public and 2 private in 2 AZ's)
    4. Create two Route tables (public for internet and private for the traffic through NAT Gateway)
    5. Create NAT Gateway
    6. ELB (Internet and the Internal Load balancer)
    7. Auto Scaling group
    8. Bastion Host

