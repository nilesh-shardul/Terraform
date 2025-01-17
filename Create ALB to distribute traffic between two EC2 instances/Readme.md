<H2> LAB DETAILS </h2>


This lab walks you through AWS Elastic Load Balancing. Elastic Load Balancing automatically distributes incoming application traffic across multiple Amazon EC2 instances in the cloud. In this lab, we will demonstrate elastic load balancing with 2 EC2 Instances using Terraform.


<H2> INTRODUCTION </h2>
<h3> What is Elastic Load Balancing? </h3>

<ol>			
	<li>	ELB is a service that automatically distributes incoming application traffic and scales resources to meet traffic demands.	</li>
	<li>	ELB helps in adjusting capacity according to incoming application and network traffic.	</li>
	<li>	ELB can be enabled within a single availability zone or across multiple availability zones to maintain consistent application performance.	</li>
	<li>	ELB offers features like:	</li>
	<li>	Detection of unhealthy EC2 instances.	</li>
	<li>	Spreading EC2 instances across healthy channels only.	</li>
	<li>	Centralized management of SSL certificates.	</li>
	<li>	Optional public key authentication.	</li>
	<li>	Support for both IPv4 and IPv6.	</li>
	<li>	ELB accepts incoming traffic from clients and routes requests to its registered targets.	</li>
	<li>	When an unhealthy target or instance is detected, ELB stops routing traffic to it and resumes only when the instance is healthy again.	</li>
	<li>	ELB monitors the health of its registered targets and ensures that the traffic is routed only to healthy instances.	</li>
	<li>	ELB's are configured to accept incoming traffic by specifying one or more listeners. A listener is a process that checks for connection requests.	</li>
	<li>	Listeners are configured with a protocol and port number from the client to the ELB and vice-versa i.e., back from ELB to the client.	</li>
	<li>	ELB supports 3 types of load balancers: 1. Application Load Balancers 2. Network Load Balancers 3. Classic Load Balancers	</li>
	<li>	Each load balancer is configured differently.	</li>
	<li>	For Application and Network Load Balancers, you register targets in target groups and route traffic to target groups.	</li>
	<li>	For Classic Load Balancers, you register instances with the load balancer.	</li>
	<li>	AWS recommends users to work with the Application Load Balancer to use multiple Availability Zones because if one availability zone fails, the load balancer can continue to route traffic to the next available one.	</li>
	<li>	We can have our load balancer be either internal or internet-facing.	</li>
	<li>	The nodes of an internet-facing load balancer have Public IP addresses, and the DNS name is publicly resolvable to the Public IP addresses of the nodes.	</li>
	<li>	Due to the point above, internet-facing load balancers can route requests from clients over the Internet.	</li>
	<li>	The nodes of an internal load balancer have only Private IP addresses, and the DNS name is publicly resolvable to the Private IP addresses of the nodes.	</li>
	<li>	Due to the point above, internal load balancers can only route requests from clients with access to the VPC for the load balancer.	</li>
	<li>	Both internet-facing and internal load balancers route requests to your targets using Private IP addresses.	</li>
	<li>	Your targets do not need Public IP addresses to receive requests from an internal or an internet-facing load balancer.	</li>
</ol>			

<h3> What is Terraform? </h3>

<ol>			
	<li>	It is an open-source IaaC (Infrastructure as a Code) software tool where you define and create resources using providers in the declarative configuration language example JSON. 	</li>
	<li>	With Terraform, You can package and reuse the code in the form of modules. 	</li>
	<li>	It supports a number of cloud infrastructure providers such as AWS, Azure, GCP, IBM Cloud, OCI, etc.  	</li>
	<li>	Terraform has four major commands: 	</li>
	<li>	terraform init 	</li>
	<li>	terraform plan 	</li>
	<li>	terraform apply 	</li>
	<li>	terraform destroy 	</li>
			
</ol>			


			

<h3> Prerequisites </h3>

<ol>			
	<li>	Install Terraform in your local machine using this official guide by Hashicorp. 	</li>
	<li>	To install Terraform using CLI, use this guide https://learn.hashicorp.com/tutorials/terraform/install-cli 	</li>
	<li>	To install Terraform by downloading, use this guide https://www.terraform.io/downloads.html 	</li>
	<li>	Download and Install Visual Studio Code editor using this guide https://code.visualstudio.com/download 	</li>	
			
</ol>			

<H2> ARCHITECTURE DIAGRAM </h2>

![architecture diagram](https://github.com/user-attachments/assets/d288c6b2-7a94-4ff6-a8fe-26eb29ce4cba)


<h2> TASK DETAILS </h2>

<ol>			
	<li>	Sign in to AWS Management Console	</li>
	<li>	Setup Visual Studio Code.	</li>
	<li>	Create a Variables file.	</li>
	<li>	Create EC2, ELB and its components in main.tf file	</li>
	<li>	Create an Output file.	</li>
	<li>	Confirm the installation of Terraform by checking the version.	</li>
	<li>	Apply Terraform configurations.	</li>
	<li>	Check the HTML page and traffic distribution.	</li>
	<li>	Check the resources in AWS Console.	</li>
	<li>	Deleting AWS Resources	</li>
<ol>			






