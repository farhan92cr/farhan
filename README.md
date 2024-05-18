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


kubernetes controls and
fix the damage so it will either control or it will fix
so most of the time it will control the damage now what is the meaning of controlling the damage or what is the



Day-31 | KUBERNETES ARCHITECTURE USING EXAMPLES:

kubernetes offers four fundamental
advantages over Docker that is
kubernetes is by default a cluster in
nature or cluster in Behavior then
kubernetes offer something called as
Auto healing kubernetes offer something
called as Auto scaling and finally it
offers multiple Enterprise level support
like kubernetes offers you Advanced load
balancing kubernetes offers you you know
security related things it offers you
Advanced networking so it offers you
multiple Enterprise level support which
is a major difference between Docker and
kubernetes 



kubernetes architecture has something called asa control plane
and kubernetes has something called as data plane.

here are multiple components in
com control plane like you know
kubernetes has uh API server kubernetes
has a component that is called as etcd
kubernetes has a component that is
called as a scheduler
then you have a controller manager and
then you have a cloud controller manager
which is called as CCM and similarly in
data plane also you have multiple
components like you know you have your
kubelet you have your proxy you have
your uh you know container runtime


Docker the simplest
thing is container whereas in kubernetes
the simplest thing is POD



Day-33 | KUBERNETES PODS | DEPLOY YOUR FIRST APP:

kubectl is to interact kubernets.
KubeCtL is nothing but like for Docker whenever you are trying to run any commands you have the docker CLI
right in kubernetes you have something called as kubectl so kubectl is command line.



For the installation of Kubernetes we need to install the follwing

1. kubectl ---> google -kubectl installation --->
   curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   kubectl version --> to verify installtion or check verion.

2. Now we will install kubernetes local cluster like
   minikube, k3s, kind, microk8s etc
   but we will install minikube. bcz it easy. kind is advanced topics, kind is basically kubernetes in docker.
   --> google --> minikube  --> select system configuration --> curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64
   
   minikube  --> to verify installtion

minikube is  command line tool which allow you create kubernetes cluster.

minikube start --> with this command kubernetes cluster will be started.

kubectl get nodes --> you see that kubectl alreday connected to kubernetes cluster.



POD :

vim pod.yml
apiVersion: v1
kind: Pod
metadata:
  name: nginx
spec:
  containers:
  - name: nginx
    image: nginx:1.14.2
    ports:
    - containerPort: 80

This is a sample yaml file, it's stay the same, we just need to change the value of keys like image: nginx:1.14.2 --> we use othe application/image instead of nginx
maybe we also chnage the container port.

docker run -d image: nginx:1.14.2 --name nginx -p 80:80 ---> if we compare a pod to docker, this the equilavent command in docker for container as the above is for Pod in kubernetes.


kubctl create -f pod.yml --> to create the pod from yaml file, we write above.
kubectl get pods --> to shows pod as in docker (docker ps)
kubectl get pods -o wide --> to shows pod in more details
curl <pod ip> --> to login to the pod application --> get ip of pod above
minikube ssh <ip>
kubectl delete pod <name like ngnix>
kubectl describe pod ngnix
kubectl log <pod name>

kubectl get all

minikube ssh --> to enter/login to a pod 
curl <ip of pod>  ---> to check if our pod is running

below demo
farhan@farhan-VirtualBox:~/kubernetes$ minikube ssh
docker@minikube:~$ curl 10.244.0.9   ----> run from the inside of a pod
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>

ssh -i <node name and ip>

kubectl cheatsheet --> google it get all kubernetes command, no need to remember all




Day-34 | KUBERNETES DEPLOYMENT | REPLICASETS :



Docker                 Pod                      Deploy:  1. auto healing  2. auto scaling

we must create pod using deployment. bcz pod like docker conatiner, no auto heling scaling etc.


deployment is responsible for implementing auto healing(recreating pods if someone delete them) and zero down time in kubernetes, 
deployment will not do it directly, but take help of replicaset, and replica set is kubernetes controller. which is actually doing it.
kubernete is a nothing but a go language application that  of kubernetes is return, which will ensure that a specific behaviour is implementtd.
the behaviour is that the desired number of state/replicas will be there in deployment.

vim deployment.yml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80



kubectl apply -f deployment.yml


   kubectl get deploy
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
nginx-deployment   3/3     3            3           5m25s
farhan@farhan-VirtualBox:~/kubernetes$ kubectl get rs   ---> rs means replicaset
NAME                          DESIRED   CURRENT   READY   AGE
nginx-deployment-77d8468669   3         3         3       5m31s
farhan@farhan-VirtualBox:~/kubernetes$ kubectl get replicaset
NAME                          DESIRED   CURRENT   READY   AGE
nginx-deployment-77d8468669   3         3         3       5m43s
farhan@farhan-VirtualBox:~/kubernetes$
kubectl get pod
NAME                                READY   STATUS    RESTARTS      AGE
nginx                               1/1     Running   2 (13m ago)   23h
nginx-deployment-77d8468669-gxjm4   1/1     Running   0             6m25s
nginx-deployment-77d8468669-lpszk   1/1     Running   0             6m25s
nginx-deployment-77d8468669-mxxpz   1/1     Running   0             6m25s
farhan@farhan-VirtualBox:~/kubernetes$

kubectl pods -w  --> to watch live 

kubectl delete pod <name>

Means if we delete/terminat a pod the recreation occur will be in the same time/parallel. bcz kubernete replicasset will ensure there will always be the number repliaset. if we delete one pod in parallel one willl recreate by kubernetes coontroller.

So in real world you cannot create pod directly, but will creata deployment, so deployment will create replicaset, rs will create pods

in conculusion, deploy create replica sets and replicaset creates pods


DAY-35 | EVERYTHING ABOUT KUBERNETES SERVICES | DISCOVERY | LOAD BALANCING | NETWORKING::

 https://www.youtube.com/watch?v=xY6Ic7Igzck&list=PLdpzxOOAlwvIKMhk8WhzN1pYoJ1YU8Csa&index=42&ab_channel=Abhishek.Veeramalla

Pod --> Deployment --> service

what if there is no service in kubenetes?

so when a pod is down for somereason, rs will create another in parallel with down one. but the problem is that the IP has changed. so the rs will healed the pod but the ip has changed. here the services concept will come. service provide load balancing.
like --> payment.default.svc --->
so user access to service, service will give the pod addres(ip).

Service  ---> 1. load blancing
              2. service discovery ---> svc alo face ip addres issue when a pod goes down, so here service use label and selectors. svc dosen't care about ip addres but use labels and selectors. label is common for all the pods. means when a pod down it auto heal, the ip addres changed but pod label will be same.
              so this is the servics discovery mechanism of kubernetes.

         Simply we add label in deployment like 
         label:
           app: payment

        so whenever a new pod is created, service will keep track of label.
              3. Expose to external world: service expose our application or service can allow our app to the external world. 
              we can create 3 type of service
              i. cluster ip --> only accessible inside cluster
              ii. Nodeport --> it will allow our app to be accessible inside our organization.   
              iii. Load balancer ---> here service will expose the app to external world.   like EKS ---> ELB(elastic load blanncer) ip --> uses public addres.


 CCM --> cloud controller manager: The kubernetes master node has CCM. CCM will genertae the public ip addres. 
 if you create a loaderblancer type then anybody can access.
 if you create nodeport type node, anybody who have the worker node access can access.
 cluster IP mode --> no body can access, only you can login kubernetes.




Day-36 | KUBERNETES INTERVIEW QUESTIONS PART-1| What's Your Score ? |10/10:





![image](https://github.com/farhan92cr/farhan/assets/120403028/c75b1fc3-83b2-4041-8119-d55f7f787fa2)

![image](https://github.com/farhan92cr/farhan/assets/120403028/426fc940-362a-487b-9870-c29887fd084c)

![image](https://github.com/farhan92cr/farhan/assets/120403028/0170ee2f-1cdf-4a0f-8e17-e520a21842fb)

![image](https://github.com/farhan92cr/farhan/assets/120403028/2a829ea3-0aeb-4e68-a92e-3b5d5f10852b)

![image](https://github.com/farhan92cr/farhan/assets/120403028/ac30696c-1a57-441f-a70d-c0425cfc6248)

 


DAY-37 | KUBERNETES SERVICES DEEP DIVE| LIVE DEMO | LEARN TRAFFIC FLOW USING KUBESHARK:

https://www.youtube.com/watch?v=fCX8O7GA_lY&t=79s&ab_channel=Abhishek.Veeramalla

minukube status
kubectl get all ---> to show all

clone https://github.com/farhan92cr/Docker-Zero-to-Hero
we will do deplyoment now.

cd example
ls
vim Dockerfile --> the exsiting one
docker build -t farhan/python-sample-app-demo:v1 .

kubernetes deployment ----> search on google  --> get the sample deployment script.

vim deployment.yml

apiVersion: apps/v1
kind: Deployment
metadata:
  name: sample-python-app
  labels:
    app: sample-python-app
spec:
  replicas: 2
  selector:
    matchLabels:
      app: sample-python-app
  template:
    metadata:
      labels:
        app: sample-python-app
    spec:
      containers:
      - name: python-app
        image: python-sample-app-demo:v1
        ports:
        - containerPort: 8000




kubectl apply -f deployment.yml

kubctl get deploy
OR
kubectl get pod

kubectl get podds -o wide --> to get IP addres

kubectl get pods -v=9 ---> v is for verbosity(get more info), can be 1 to 9. 9 is highest


kubectl delete pod <name>





              
                






 
