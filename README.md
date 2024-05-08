AWS Zero Hero day 1:

What is DevOps:
I would say devops is a process of improving the application delivery by ensuring there is a proper automation with a code quality that is maintained or with the application quality that is maintained and ensuring there is a continuous monitoring and continuous testing in place. 
Four pillars of devops are:
1. automation
2. quality
3. monitoring 
4. testing

AWS Zero Hero day 2:
Software Development lifecycle:(SDLC)
software development lifecycle is a process that is followed by the industry to design
develop and test high quality product.


AWS Zero Hero day 13: 

AWS Services that Every DevOps Engineers should learn.

1.  EC2 --> Live Project
2.  VPC --> Virtual Private Cloud -->  securing your AWS resources we use VPC, like ec2 instance, Cidr block, inbound traffic rules
3.  EBS --> Volume --> we need to know how attach a volum with EC2 instance. --> EC2 has by default storage,
    it better to store the information into volume mounts, so we can easiy attach, deattach them.
4. S3 --> (Storage) , it save file and folder like google drive.
5. IAM  user --> (identity and access managemnet) --> the aws service that takes care of identity and access management is AWS IAM.
6. Cloud watch --> cloudwatch takes care of monitoring and observing
7. Lambda -->
   now coming to Lambda like I told it's a serverless computer now what is the difference between Lambda and ec2 if I am
   saying that using Lambda I can execute some action and I am calling it serverless whereas ec2 is by default a compute service which has a server
   what is the difference so the difference here is that AWS Lambda functions you know they can be created and paid on automatically
   like you don't have to do anything from your end like for example you go ahead and create a ec2 instance from the AWS console but whenever
   you want to use AWS Lambda you can directly like you know run the program or you know you can execute your Lambda function and AWS
   will automatically okay even without your request like you it will not ask you do you want a Ubuntu underneath or do you
   want for example do you want a red hat or you want send OS what AWS will do is it will take your action it will take your
   code automatically it will create an instance for you it will execute the code on the instance and once the execution is done it will tear down
   the instance okay so Lambda are serverless computes which are used for short actions okay unless you're easy to instance in your
   ec2 instance what you'll do you will deploy your application whereas Lambda are used for executing this short what actions or this short
   functionalities that can be teared on and like you know executed and teared on automatically.
   

8. Cloud Build Services
   - Aws code piplines --> it's like jenkins pipline
   - Aws code build    --> it is a fully managed build service that takes care of
                           compiling your code okay run some tests and provide some
                           software packages.
   - Aws code deploy   --> code deploy takes care of deploying your code or you know deploying your applications
                           onto ec2 instances or on-premises servers okay so let's take an example for example you have your application let's say it's a legacy application or it's a micro service it is not containerized it it is being deployed on your ec2 instances for now so there has to be a set Easy Way by which once your artifacts are built okay once your continuous integration is done and let's say you have your artifact uh it can be a jar file War file or something let's say there is a war file that is created by your continuous integration and you want to deploy this war file onto a ec2 instance okay so that whoever is the user is getting the latest version of your ec2 uh sorry of your application on ec2 instance so for it to automatically happen you can use your AWS code deploy and code build like I mentioned you it takes care of your build related service okay uh whatever you are compiling of your code is a running of your code and all of these things and code pipeline is like your uh very similar to your Jenkins pipeline so these are the things and these are the tools using which AWS cicd takes place so if you are on AWS completely or if your organization is on AWS completely so you have to reevaluate why you are using Jenkins is it because you have Jenkins from old times or you know uh have you been using Jenkins uh for a long time now and it is difficult to migrate to AWS uh code related build related Services if if that is the case then you know you have to rethink okay because I'm completely on AWS now do I want to move completely to these things or in future I might move from AWS to Azure if you are in that certain State definitely.

9. Aws Configuration:  --> AWS configuration service you can basically go ahead and look what are the configurations you have created like the basic example that I previously stated uh somebody is creating a unencrypted EBS volume or somebody is creating a S3 bucket without worsening so you know you can configure all of these things in your configuration AWS configuration and you can perform some remedy action 


10. Billing and costing related services:

11. AWS KMS:  --> Key Management Service
    Key Management Service that means if you have some Secrets uh you have some Certificate Management certificates that you want to rotate or
    you know certificates that you want to manage okay so in such cases you can store these certificates or you can store this kind of sensitive
    information in AWS KMS and using KMS you can do things sort of service integration you can do sort of uh you know certificates rotation.

12. Cloudtrail -->
    it is a service you understand it as something that records here API activities okay and it preserves logs for a specific duration
    like you know using cloudtrail you get you can get logs for uh last 30 days last six months so this is why cloud trail is used.

13. Elastic Kubernetes Service --> AWS offers a managed kubernetes service.

14. Fargate and ECS --> these are  aws container services.


15. ELK ---> Elasticsearch one of the better combinations is to use log stash and kibana

16.  ML (machine Learning)



AWS Zero Hero day 14:
       Configuration Management With Ansible:

       1. Upgrades
       2. Secure patches
       3. installation

configuration management will aim to solve the problem of config or managing the configuration of multiple servers. 
Configuration Management tools are 
 1. Puppet   ---> push model --- puppet language ---new language
 2. chef
 3. ansible  ---> pull model --- agentless --- yaml --> global language
 4. salt


AWS Zero Hero day 16:
   Infrastructure as Code | Terraform #IaC  : 
   Terrafrom is also a API as code. ---> talk to any service provider using thier API

what is api code so API as code
is a concept using which you can
automate any provider whether it is AWS
Azure or gcp anything using their
apis okay so what terraform does
internally is terraform will talk to the
API of azure terraform will talk to the
API of gcp or terraform will talk to the
API of openstack so using which like you
know you don't have to write any code so
once you write the terraform templating
or you write the terraform script files
terraform will convert them depending
upon the provider details that you have
provided so in one of the files called
provider.tf you say that the provider is
AWS so once you write the terraform
module terraform will convert that
script into AWS readable API okay or the
API request that AWS can understand and
it executes the action and gives you the
result back okay so this is how
terraform is one tool that can automate
your resources on any cloud provider.




























   
