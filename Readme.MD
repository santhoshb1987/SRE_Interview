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


# Orchestration Tools:
Docker
Kubernetes

# IaaC Tools
Terraform

# Configuration Management Tools
Ansible 

# Operating System
Linux


# Operations:
Observability 
- Prometheus 
- Otel Monitoring
- Google Stack Driver logging 
- Alerting 

# Oncall 
Pagerduty/Slack Integration
oncall rotation 
RCA
Post Mortem 

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
- GitOps

