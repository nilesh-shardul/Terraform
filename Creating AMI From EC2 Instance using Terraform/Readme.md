<H2> LAB DETAILS </h2>


This lab walks you through the steps to create an AMI from EC2 Instance using Terraform and launching new EC2 Instance using that AMI.

<H2> INTRODUCTION </h2>
<h3> What is AMI ? </h3>

<ol>			
	<li>	AMI stands for Amazon Machine Image. 	</li>
	<li>	It's a master image for the creation of virtual servers i.e., EC2 instances in the AWS environment. 	</li>
	<li>	They are like templates that are configured with an operating system and other software, which determine the user's operating environment. 	</li>
	<li>	AMIs are categorized according to region, operating system, system architecture (32 or 64 bit), launch permissions and whether they are backed by Amazon EBS or by the Instance Store. 	</li>
	<li>	AMI includes a template for the root volume required for an instance; typical example might contain an operating system, an application server and applications. 	</li>
	<li>	When you launch an instance, the root device volume contains the image used to boot the instance. 	</li>
	<li>	In the initial stages, all AMIs were backed by the Amazon EC2 Instance Store. This means the root device for an instance launched from the AMI is an Instance Store volume created from a template stored in Amazon S3. 	</li>
	<li>	Any data on the instance store volumes persists as-long-as the instance is running i.e., the data gets deleted once the instance is terminated. 	</li>
	<li>	Instance store backed instances do not support the Stop action. 	</li>
	<li>	If using an instance store is required, Amazon recommends distributing the data across multiple Availability Zones. 	</li>
	<li>	After the introduction of Amazon EBS, Amazon introduced AMIs that are backed by Amazon EBS i.e., the root device for an instance launched from the AMI is an Amazon EBS volume created from an EBS Snapshot. 	</li>
	<li>	Amazon recommends using EBS backed AMIs, because they launch faster and use persistent storage. 	</li>
	<li>	Amazon EBS backed instances can be stopped and later restarted without affecting data stored in the attached volumes. 	</li>
	<li>	Permissions are controlled to constrain AMIs for instance launches to the appropriate AWS accounts. 	</li>
			
</ol>			

<H2> What is Terraform? </h2>

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





<h2> TASK DETAILS </h2>

<ol>			
	<li>	Sign in to AWS Management Console 	</li>
	<li>	Setup Visual Studio Code. 	</li>
	<li>	Create a Variables file. 	</li>
	<li>	Create EC2and it’s AMI in main.tf file 	</li>
	<li>	Create an Output file. 	</li>
	<li>	Confirm the installation of Terraform by checking the version. 	</li>
	<li>	Apply Terraform configurations. 	</li>
	<li>	Check the resources in AWS Console. 	</li>
	<li>	Launching the EC2 instance with the created AMI using terraform. 	</li>
	<li>	Deleting AWS Resources. 	</li>
			
</ol>			

  



