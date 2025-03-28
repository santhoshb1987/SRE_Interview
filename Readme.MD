# SRE Interview for GCP

# Programming Interview:

Python Coding 

https://www.geeksforgeeks.org/python-interview-questions/
1. What is indentation?
```
Yes, indentation is required in Python. A Python interpreter can be informed that a group of statements belongs to a specific block of code by using Python indentation.
```
2. Statically typed/Dynamically Typed
```
Programming Languages can be divided into the following two types.

Statically typed languages: In this type of language, the data type of a variable is known at the compile time which means the programmer has to specify the data type of a variable at the time of its declaration. Examples are C, C++, Java and C#
Dynamically typed languages: These are the languages that do not require any pre-defined data type for any variable as it is interpreted at runtime by the machine itself. In these languages, interpreters assign the data type to a variable at runtime depending on its value. Examples are Python and JavaScript
```

3. How do you floor a number in Python?
```
import math

n = 3.7
F_num = math.floor(n)
print(F_num) 
```

4. What is a pass in Python?
```
Pass statement in Python is a null operation or a placeholder.
```

5. What is a lambda function?
```
A lambda function is an anonymous function. 
This function can have any number of parameters but, can have just one statement.


s1 = 'GeeksforGeeks'

s2 = lambda func: func.upper()
print(s2(s1))
```
6. How is a dictionary different from a list?
```
A list is an ordered collection of items accessed by their index, while a dictionary is an unordered collection of key-value pairs accessed using unique keys. 
Lists are ideal for sequential data, whereas dictionaries are better for associative data. 
For example, a list can store [10, 20, 30], whereas a dictionary can store {“a”: 10, “b”: 20, “c”: 30}.
```

7. What is the difference between a Mutable datatype and an Immutable data type?
```
Mutable data types can be edited i.e., they can change at runtime. Eg – List, Dictionary, etc.
Immutable data types can not be edited i.e., they can not change at runtime. Eg – String, Tuple, etc.
```
8. What is List Comprehension? Give an Example.
```
List comprehension is a way to create lists using a concise syntax. It allows us to generate a new list by applying an expression to each item in an existing iterable (such as a list or range).

a = [2,3,4,5]
res = [val ** 2 for val in a]
print(res)
```
9. What are *args and **kwargs?
```
*args: The special syntax *args in function definitions is used to pass a variable number of arguments to a function. Python program to illustrate *args for a variable number of arguments:

def myFun(*argv):
    for arg in argv:
        print(arg)

myFun('Hello', 'Welcome', 'to', 'GeeksforGeeks')

Output
Hello
Welcome
to
GeeksforGeeks
```

```
**kwargs: The special syntax **kwargs in function definitions is used to pass a variable length argument list. We use the name kwargs with the double star **.


def fun(**kwargs):
    for k, val in kwargs.items():
        print("%s == %s" % (k, val))
# Driver code
fun(s1='Geeks', s2='for', s3='Geeks')

Output
s1 == Geeks
s2 == for
s3 == Geeks
```
10. What is the difference between a Set and Dictionary?
```
A Python Set is an unordered collection data type that is iterable, mutable and has no duplicate elements.

my_set = {1, 2, 3}
```
Dictionary in Python is an ordered (since Py 3.7) [unordered (Py 3.6 & prior)] collection of data values, used to store data values like a map, which, unlike other Data Types that hold only a single value as an element, Dictionary holds key:value pair.
```
my_dict = {“a”: 1, “b”: 2, “c”: 3}
```
11. Differentiate between List and Tuple?

```
List

Lists are Mutable datatype.
Lists consume more memory
The list is better for performing operations, such as insertion and deletion.
The implication of iterations is Time-consuming
Tuple

Tuples are Immutable datatype.
Tuple consumes less memory as compared to the list
A Tuple data type is appropriate for accessing the elements
The implication of iterations is comparatively Faster
```
12. Write a code to display the current time?
```
import time

currenttime= time.localtime(time.time())
print ("Current time is", currenttime)
```


# Cloud:
Google Cloud

https://medium.com/@thecloudarchitect/my-devops-notes-for-gcp-scenario-based-interview-questions-with-answer-e71381c22afa
https://www.igmguru.com/blog/gcp-interview-questions

1. How do you manage secrets in GCP?
```
Ans: Manage secrets in GCP using Secret Manager. Store sensitive information such as API keys, passwords, and tokens securely.
```
2. How do you monitor applications in GCP?
```
Ans: Monitor applications in GCP using Google Cloud’s operations suite, including Cloud Monitoring, Cloud Logging, and Cloud Trace. Set up metrics, create dashboards, configure alerts, and analyze logs to ensure the health and performance of your applications.
```
3. How do you implement blue-green deployments in GCP?
```
Ans: Implement blue-green deployments in GCP by setting up two identical environments. Deploy the new version to the blue environment, test it, and switch traffic from the green (current production) environment to the blue environment using Cloud Load Balancer or DNS updates.
```
4. How do you secure a GKE cluster?
```
Ans: Secure a GKE cluster by implementing best practices such as enabling private clusters, using network policies to control traffic, setting up role-based access control (RBAC), enabling binary authorization for container images, and regularly updating the cluster and node software.
```
5. How do you set up network security in GCP?
```
Ans: Set up network security in GCP by configuring VPCs, subnets, firewall rules, and Cloud Armor policies. Use Identity-Aware Proxy (IAP) to control access to your applications, and implement secure access using VPNs or Cloud Interconnect.
```
6. How do you use Stackdriver Logging in GCP?
```
Ans: Use Stackdriver Logging (now part of Cloud Logging) to collect and analyze logs from your applications and GCP services. Create log-based metrics, set up alerts, and use log sinks to export logs to BigQuery or Cloud Storage for further analysis.
```
7. How do you handle disaster recovery in GCP?
```
Ans: Handle disaster recovery in GCP by implementing backup and restore strategies using Cloud Storage, Cloud SQL, and other managed services. Use multi-region storage for data redundancy, set up failover mechanisms, and test your disaster recovery plans regularly.
```
8. How do you manage service accounts in GCP?
```
Ans: Manage service accounts in GCP by creating service accounts for applications and services that need to access GCP resources. Assign appropriate IAM roles to service accounts, and use service account keys for authentication when necessary. Rotate keys regularly and follow the principle of least privilege.
```
9. How do you use Cloud Scheduler in GCP?
```
Ans: Use Cloud Scheduler to trigger jobs at specified times or intervals. Schedule tasks such as HTTP requests, Pub/Sub messages, or Cloud Functions executions
```

10. How do you secure data in transit and at rest in GCP?
```
Ans: Secure data in transit by using TLS/SSL for communication between services and encrypt data at rest using Cloud KMS for key management. Enable encryption for storage services like Cloud Storage, BigQuery, and Cloud SQL, and manage encryption keys with IAM policies.
```

# Orchestration Tools:
Docker

https://www.linkedin.com/pulse/day-21-docker-important-interview-questions-kartik-bhatt-xp5pc

Learning Tutorial: https://www.simplilearn.com/tutorials/docker-tutorial

Kubernetes
https://www.geeksforgeeks.org/kubernetes-interview-questions/

1. Explain Kubernetes Architecture?
```
Kubernetes is an open-source container deployment and administration platform. It offers container orchestration, container runtime, container-centric infrastructure orchestration, balance of load, self-healing mechanisms, and service discovery. A Kubernetes cluster has several control planes and one or more worker nodes.
```
2. What is a Pod in Kubernetes?
```
A cluster of one or more Linux containers makes up a Kubernetes pod, the smallest unit of a Kubernetes application.
```
3. What is Kubelet?
```
Kubelet is an important component of Kubernetes that manages containers within pods on a node. It registers the node with the control plane and provides resource information. Kubelet keeps an eye on container health and responds to problems—lik isnces of pods that contain a containerized application.
```
4. What is a Service in Kubernetes?

```
The idea of the Service is to group a set of Pod endpoints into a single resource. We can configure various ways to access the grouping. By default, we can get a stable cluster IP address that the clients inside the cluster can use to contact Pods in Service.

apiVersion: v1
kind: Service
metadata:
name: my-service
spec:
    selector:
        Tomcat: deploymentapp
    ports:
        - protocol: TCP
          port: 80
          targetPort: 8080
```
5. 


# Version Control Tools
Git
1. What is the difference between git fetch and git pull?
```
The main difference between git fetch and git pull lies in what they do and how they update the local repository.

The git fetch command retrieves changes from a remote repository to the local repository. It updates the remote-tracking branches (e.g., origin/master) in the local repository to reflect the state of the remote repository, but it does not update the working directory or merge any changes into the current branch. This means that after fetching, you can review the changes made in the remote repository without affecting your local work.

The git pull command also retrieves changes from a remote repository, but it goes a step further by fetching changes and merging them into the current branch in one step. It essentially performs a git fetch followed by a git merge to incorporate the changes from the remote repository into the current branch.
```
2. How do you revert a commit that has already been pushed and made public?
```
The git revert <commit-hash> command can be used to revert a commit.
Identify the commit you want to revert to by finding its commit hash. This can be done using the git log command to view the commit history and find the commit hash you want to revert.
Once you have the commit hash, use the git revert command followed by the commit hash to create a new commit that undoes the changes introduced by the specified commit. For example:

git revert <commit-hash>
```
3. What does git reset do?
```
The git reset command resets the current HEAD to a specified state. This means it can be used to undo changes, unstage files, or move the HEAD pointer to a different commit.
```

4. What is git stash?
```
git stash is a Git command that temporarily stores changes in the working directory that are not ready to be committed. It allows developers to save their modifications without committing them to the repository.
```

5. What is the use of git submodule and how do you update one?
```
The git submodule command manages external dependencies within a Git repository. It allows you to include external repositories as submodules within your main repository. This is useful when you want to incorporate code from external sources while keeping it separate from your main project's codebase.
```
6. Can you name some deployment strategies?
```
Regular release/deployment: releases software to everyone at once, making it available to the general public.

Canary releases: this is a method that reduces the chance of failure by exposing a small portion of the userbase (around 1%) to the release. With a canary release, developers gradually switch users to the latest release in a controlled way.

Blue-green releases: consists of running two simultaneous instances of an application; one is the stable version currently serving users and the other the latest release. Users are switched from the former to the latter all at once. This method is safer than the regular or big bang releases because users can instantly be routed back to the previous version if there is a problem.

Dark launches: are deployments where new features are released without being announced. Features can be enabled in a very fine-grained way with feature flags.
```
# IaaC Tools

Terraform
https://www.geeksforgeeks.org/terraform-interview-questions/

1. What are the most useful Terraform commands?
```
terraform init — Initializes the current directory, also Plugin Installation, Module Installation, Backend Initialization, and Version Checking is done in the background.
terraform refresh — Terraform compares the current state of your infrastructure with the state described in your Terraform configuration files and updates its state file accordingly.
terraform output — Retrieve the values of output variables defined in your Terraform configuration.
terraform apply — Terraform to apply the changes described in your Terraform configuration files to your infrastructure.
terraform destroy — Terraform is used to destroy all the resources defined in your Terraform configuration.
terraform graph — Creates a DOT-formatted graph
terraform plan — Terraform is used to generate an execution plan based on your Terraform configuration files.
```
2. Question 1: You have an existing infrastructure on AWS, and you need to use Terraform to manage it. 

How would you import these resources into your Terraform configuration?
We can use the terraform import command, we need to create a configuration file (dummy file)
```
terraform import [OPTION] ADDRESS_ID 

terraform import aws_instance.localname i-abcd123 
```
3. Question 2: You are working with multiple environments (e.g., dev, prod) and want to avoid duplicating code. How would you structure your Terraform configurations to achieve code reuse?
```
We make use of modules so that we can avoid duplication of code.

terraform workspace list #To list all workpace 

terraform workspace new dev 
terraform workspace new prod

Switching Between Workspaces 

terraform workspace select <workspace_name> 
```

4. Question 3: Describe a situation where you might need to use the terraform remote backend, and what advantages does it offer in state management?
```
Benefits: Shared state, locking, secure state storage.
```

5. Question 4: You need to create a highly available architecture in AWS using Terraform. Explain how you would implement an Auto Scaling Group with load balancing.
```
Define Load Balancer Resources:
resource "aws_lb" "example" {
  name               = "example-lb"
  internal           = false
  load_balancer_type = "application"

  security_groups    = ["${aws_security_group.example.id}"]

  subnets            = ["${aws_subnet.example.id}"]
}


resource "aws_lb_target_group" "example" {
  name        = "example-tg"
  port        = 80
  protocol    = "HTTP"
  target_type = "instance"

  health_check {
    path                = "/"
    interval            = 30
    timeout             = 5
    healthy_threshold   = 2
    unhealthy_threshold = 2
  }

  vpc_id = "${aws_vpc.example.id}"
}
Define Auto Scaling Group:
resource "aws_autoscaling_group" "example" {
  name                 = "example-asg"
  min_size             = 2
  max_size             = 5
  desired_capacity     = 2
  vpc_zone_identifier  = ["${aws_subnet.example.id}"]

  target_group_arns = ["${aws_lb_target_group.example.arn}"]
}
Attach ASG to Load Balancer:
resource "aws_autoscaling_attachment" "example" {
  autoscaling_group_name = "${aws_autoscaling_group.example.name}"
  alb_target_group_arn   = "${aws_lb_target_group.example.arn}"
}

```
6. Question 5: Your team is adopting a multi-cloud strategy, and you need to manage resources on both AWS and Azure using Terraform. How would you structure your Terraform code to handle this?
Organize Directories by Cloud Provider:
```
terraform_project/
├── aws/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
├── azure/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
└── modules/
    ├── aws_module/
    │   ├── main.tf
    │   ├── variables.tf
    │   ├── outputs.tf
    ├── azure_module/
    │   ├── main.tf
    │   ├── variables.tf
    │   ├── outputs.tf
```

# Configuration Management Tools

Ansible 
https://www.interviewbit.com/ansible-interview-questions/
https://k21academy.com/devops-job-bootcamp/ansible-interview-questions-and-answers/

1. What is idempotence in Ansible?
```
Idempotence in Ansible refers to the ability of tasks to be executed multiple times without changing the result beyond the initial execution, ensuring consistent outcomes.
```
2. What are Ansible ad-hoc commands?
```
Ansible ad-hoc commands are one-liners used to perform simple tasks without writing playbooks. They are executed from the command line and allow tasks like running shell commands or restarting services.
```
3. How do you handle errors in Ansible playbooks?
```
Ansible provides mechanisms for error handling, including the ignore_errors directive, failed_when condition, and rescue blocks, ensuring graceful handling of errors during playbook execution.
```
4. How do you securely manage sensitive data like passwords and API keys in Ansible playbooks without using Ansible Vault?
```
Securely managing sensitive data in Ansible playbooks can be achieved using external credential management solutions like HashiCorp Vault or external password management systems.
These solutions integrate with Ansible to securely retrieve and manage sensitive information.
```

# Operating System

Linux
https://www.geeksforgeeks.org/linux-interview-questions/

# Operations:
Observability 
- Prometheus 
https://www.devopsschool.com/blog/top-50-prometheus-interview-questions-and-answers/
- Otel Monitoring
- Google Stack Driver logging /Metrics Explorer
- Alerting 

# Oncall 
Pagerduty/Slack Integration
oncall rotation 
RCA 5 Whys + Dealing with PO P1 issues/ Runbooks
Post Mortem 
slack - bot intergrations

# Database:
- Postgres
- Backup & Restore strategies 
- logging 
- Transactions/ Performamce 
- Indexing 
- Schema /permissions 
- Onprem/Managed Database Service 

# CI/CD
- FluxCD
https://github.com/fluxcd/flux2-kustomize-helm-example
- GitOps
https://cloudsoftsol.com/interview-questions/top-gitops-interview-questions-and-answers-for-devops-engineers/


# Networking
https://www.geeksforgeeks.org/computer-network-cheat-sheet/?ref=lbp

https://www.geeksforgeeks.org/tcp-3-way-handshake-process/

# Storage
SAN & NAS

NFS
SMB

Active Directory/ Domain Name/ Name Server 


https://www.acte.in/netapp-interview-questions-and-answers


