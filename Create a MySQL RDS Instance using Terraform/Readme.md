<H2> LAB DETAILS </h2>


This lab walks you through to creation and testing of Amazon RDS MySQL Database using terraform. 

<H2> INTRODUCTION </h2>
<h3> What is Terraform? </h3>

<ol>			
	<li>	It is an open-source IaaC (Infrastructure as a code) software tool where you define and create resources using providers in the declarative configuration language example JSON.	</li>
	<li>	With Terraform, You can package and reuse the code in the form of modules.	</li>
	<li>	It supports a number of cloud infrastructure providers such as AWS, Azure, GCP, IBM Cloud, OCI, etc. 	</li>
	
	<li>	terraform has four major commands: </li>	
			
				
				1. terraform init 	
				2. terraform plan 	
				3. terraform apply 	
				4. terraform destroy	
			
	
</ol>			


			

<h3> Prerequisites </h3>

<ol>			
	<li>	Install Terraform in your local machine using this official guide by Hashicorp. 	</li>
	<li>	To install Terraform using CLI, use this guide https://learn.hashicorp.com/tutorials/terraform/install-cli 	</li>
	<li>	To install Terraform by downloading, use this guide https://www.terraform.io/downloads.html 	</li>
	<li>	Download and Install Visual Studio Code editor using this guide https://code.visualstudio.com/download 	</li>
	<li>	For testing this lab, it is necessary to download the MySql GUI Tool. To download it, go to the Download MySQL Workbench page. Based on your OS, select the respective option under Generally Available (GA) Releases. Download and Install. </li>
			
</ol>			


<H2> ARCHITECTURE DIAGRAM </h2>





<h2> TASK DETAILS </h2>

<ol>			
	<li>	Sign into AWS Management Console.	</li>
	<li>	Setup Visual Studio Code	</li>
	<li>	Create a variable file.	</li>
	<li>	Create a security group for RDS Instance in main.tf file	</li>
	<li>	Create RDS Database Instance in main.tf file	</li>
	<li>	Create an output file	</li>
	<li>	Confirm the installation of Terraform by checking the version.	</li>
	<li>	Apply terraform configurations	</li>
	<li>	Check the resources in AWS Console	</li>
	<li>	Testing RDS Connection using the MySQL Workbench	</li>
			
</ol>			
		

  



