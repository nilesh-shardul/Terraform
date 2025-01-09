<H2> LAB DETAILS </h2>


This lab walks you through creating IAM Users using both the Console and Command Line Interface (CLI), followed by testing their access to an S3 bucket.

<H2> INTRODUCTION </h2>
<h3> What is IAM ? </h3>

<ol>

<li>	Stands for Identity and Access Management. </li>
<li>	Web service that helps the user securely control access to AWS resources. </li>
<li>	Used to control who is authenticated and authorized to use AWS resources. </li>
<li>	The first "identity" is the creation of an account in the AWS portal.  On providing the email and password an Identity is created, and that's the "root user" holding all the permissions to access all resources in AWS. </li>
<li>	The primary resources in IAM are users, groups, roles, policies, and identity providers. </li>
<li>    IAM Group is a collection of IAM Users. You use groups to specify permissions for a collection of users, which can make those permissions easier to manage for those users. </li>
<li>	IAM roles are like IAM Users in that they are both identities with permission policies that determine what the owner can access. </li>
<li>	IAM Role does not have any credentials associated with them. </li>
<li>	IAM Roles are intended to be assumed by anyone who needs them.</li>
<li>	IAM can be used from the AWS CLI, AWS SDK, and AWS Management Console. </li>

</ol>


<H2> ARCHITECTURE DIAGRAM </h2>



<h2> TASK DETAILS </h2>

<ol>
<li>	Sign into AWS Management Console. </li>
<li>	Creating a S3 bucket </li>
<li>	Creating an IAM User using Console </li>
<li>	Testing the IAM User </li>
<li>	Creating an environment in CloudShell </li>
<li>	Create an IAM User using CLI </li>
</ol>

  



