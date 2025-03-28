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

# IaaC Tools

Terraform
https://www.geeksforgeeks.org/terraform-interview-questions/

# Configuration Management Tools

Ansible 
https://www.interviewbit.com/ansible-interview-questions/

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


