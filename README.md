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


API: ---> concept called API okay so
using API you can programmatically talk
to any applications so whether it is
GitHub whether it is Google. using https or curl




Day-25 | Docker Containerzation for Django:

Inside a docker file the difference b/w Entrypoint and cmd is that, both are 
same used to commands but the Entrypoint command be changed. cmd will change.




Day-27 | Docker Volumes and Bind Mounts|Persistent Storage for Docker:

docker -v < >
docker --mount
both are same command used for mount of docker. just the syntax diff, it bcz --mount has more verbos options. to 
more clear undestanding for others.


Day-28 | Docker Networking | Bridge vs Host vs Overlay |Secure containers with custom bridge network:
  - Basically networking allows containers to communicate with each other and the host system.
    


Day-29 | Docker Interview Questions with Answers:

Docker add command can copy the files or you know files or whatever you are
trying to do from a specific URL let's say you want to get a log file from some
AWS S3 storage or you want to get some uh Java related file or you know any uh
text file from GitHub as a raw file okay so in such cases you can use Docker add
okay so the simple example is let's say you want to retrieve the log file from S3 bucket or you want to want to
download a specific package from internet using W gate or Cal so in some cases in such cases you can use the
docker add command once you give it the URL it will try to download whereas Docker copy is basically used to copy
the files from your file system let's say you want to copy the source code from your file system from your laptop
from your ec2 instance into the Container in such cases you will use the docker copy command so fairly different
there is no similarity between both of them people get confused when they try
to explain to the interviewer just be clear




Day-30 | KUBERNETES IS EASY | INTRODUCTION TO KUBERNETES:


Docker is a container platform that means Docker is making you the
interaction with the containers or you know Docker is making your container Journey very easy because it provides a
complete container life cycle whether it is using the docker engine or using the docker CLI it makes you the I mean it
makes your container Journey very easy but now what is kubernetes then so if you already have a container platform
and if the container platform is offering you a lot of things what is kubernetes so for the textbook
definition kubernetes is nothing but a container orchestration platform.


Ephemeral:
it is nothing but something that is short
life or you know short living in nature that means containers can die 


Four problems with docker here and let us see how kubernetes is 
solving each of this problem the first problem is a
single host second problem is Auto scaling
third problem is Auto healing
fourth problem is Enterprise level support



kubernetes solves this problem so let's try to understand by default kubernetes is a cluster
what is a cluster cluster is basically group of nodes.


kubernetes installed in a master node architecture,


kubernetes has something called as replication controller or replica sets so replica
set is a new name replication controller is old name okay just like you can consider version one and version two so
kubernetes has something called as replica set.



   
