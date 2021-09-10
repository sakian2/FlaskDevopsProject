Managing Case Sensetive
Create Drop Down where it can list all the measure unit
Add +- button to increase/decrease the temperature
Integrate with the datatbase to save all the results for every students
Can use as resstful API and make it serverless(lambda)

###########Deployment Inprovements###########
#add integration test and unit test
#Add email notification for build update in pipeline
#

########Terraform#######
#Download all the files from the terraform directory
#Create a S3 bucket and update the name of the bucket on backend.tf
#Set aws access key and secret access key on the variables.tf file
#For using the Aws default credentials profile, Use the providers.tf and remove variables.tf (default aws credentials "~./aws/credentials")
#add a new user with admin programmatic access and authenticate using the access key
#Check the version of the python image if its updated or not
#Run "terraform init"
#Run "terraform plan" & "terraform apply"
#Open Aws Elastic Beanstack & open the application.
#Access the sample app from the URL.

############Application Deployment using Aws Codepipeline#############
#
