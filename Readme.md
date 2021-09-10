# Temperature Converter

A simple flask application which can check the conversion of Celsius, Fahrenheit, Rankine & Kelvin. 

## Description

This project is made for Flexion Devops Code Challenge. This project shows how to deploy the flask application into AWS Beanstalk and create the Ci/CD pipeline using AWS CodePipeline. For provisioning the infrastructure i have used Terraform. The state will be saved into S3 bucket for future use.

## Getting Started

* Clone the terraform Repo: [TerraformElasticBeanstalk](https://github.com/sakian2/TerraformElasticBeanstalk.git)
* Create a S3 bucket and update the name of the bucket on backend.tf
* Run the terraform Script to create the stack
* Set aws access key and secret access key on the variables.tf file
* Add a new user with admin programmatic access and authenticate using the access key
* Check the version of the python image from: [Aws Elastic Beanstalk Platform releases](https://docs.aws.amazon.com/elasticbeanstalk/latest/relnotes/release-2021-09-02-linux.html#release-2021-09-02-linux.platforms.python)
* Run The following commands to create the stack using terraform
```
terraform init
terraform plan
terraform apply
```

* Open Aws Elastic Beanstack & open the application from the link.
* Access the sample app from the URL to check the successful deployment

### Dependencies

* terraform
* virtual Environment to run locally
* Flask

### Running Application Locally

* For running the flask locally you need to create virtual environment and run the application inside the environment. 
* To create the environment and run the application locally use the following commands
```
pip install pipenv
pipenv shell
pipenv install flask
pipenv install pylint
pipenv install autopep8
python application.py
```

### Deploying the application into pipeline
* Create pipeling in AWS Codepipeline
* Add source repository [awesome-readme](https://github.com/sakian2/testTempProject.git)
* Select aws Elasticbeanstalk as Stack
* Select the Environment
* Create the Pipeline and wait to deploy

### Git Info
* After Cloning the repo, Create feature branch
* Create pull request to main branch to merge the changes
* Code will be merged after the code review by the author and contributor.

## Authors

Mohius Sunnah Noor Sakian [@sakian2](https://linkedin.com/sakian2)

## Version History
* 0.1
    * Initial Release

## License

This project is not licensed yet.

## Improvements can be made Next
### Application
* Managing Case Sensetive
* Create Drop Down where it can list all the measure unit
* Add +- button to increase/decrease the temperature
* Integrate with the datatbase to save all the results for every students
* Can use resstful API with flask and make it serverless(lambda)

### Infrastructure & Deployment
* Adding integration test and unit test
* Add email notification for build update in pipeline


