# Deploying a Web Server on AWS using Terraform

So I have been working with Terraform a while which seems pretty cool and faster than the regular cloud console.
This project aims to deploy a webserver on Amazon Web Services using Terraform. The steps to achieving this will be listed below:
<ul>
<li>Create a Virtual Private Cloud (VPC)</li>
<li>Create an Internet Gateway - to send traffic out to the internet </li>
<li>Create a Custom Route Table</li>
<li>Create a Subnet</li>
<li>Associate the subnet with the created Route table</li>
<li>Create a Security group allowing ports 22(SSH),80(HTTP) and 443(HTTPS)</li>
<li>Create a network interface with an IP from the subnet created earlier</li>
<li>Assign an elastic IP to the previously created network interface</li>
<li>Create an ubuntu server and intsall/enbale apache2</li>
</ul>

To begin, we need to create a key pair so that we can connect securely by using both public and private key together
