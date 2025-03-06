Deploying a Hotstar clone—a popular streaming platform—using the principles of DevSecOps on Amazon Web Services (AWS). 
The deployment process encompasses the utilization of various tools and services, including Docker, Jenkins, Java, SonarQube, 
AWS CLI, Kubectl, and Terraform, to automate, secure, and streamline the deployment pipeline.<br>

# Step-by_step Development Process <br>
## Step 1: Setting up AWS EC2 Instance <br>
* Creating an EC2 instance with Ubuntu AMI, t2.large, and 30 GB storage.<br>
* Assigning an IAM role with Admin access for learning purposes.<br>

## Step 2: Installation of Required Tools on the Instance <br>
* Writing a script to automate the installation of: <br>
>> * Docker <br>
>> * Jenkins <br>
>> * Java <br>
>> * SonarQube container <br>
>> * AWS CLI <br>
>> * Kubectl <br>
>> * Terraform <br>

## Step 3:Jenkins Job Configuration <br>
* Creating Jenkins jobs for: <br>
>> * Creating an EKS cluster. <br>
>> * Deploying the Hotstar clone application. <br>
* Configuring the Jenkins job stages: <br>
>> * Sending files to SonarQube for static code analysis.<br>
>> * Running `npm install` <br>
>> * Implementing OWASP for security checks <br>
>> * Installing and running Docker Scout for container security. <br>
>> * Scanning files and Docker images with Docker Scout. <br>
>> * Building and pushing Docker images. <br>
>> * Deploying the application to the EKS cluster. <br>

## Step 4: Clean-Up Process
* Removing the EKS cluster. <br>
* Deleting the IAM role. <br>
* Terminating the Ubuntu instance. <br>

