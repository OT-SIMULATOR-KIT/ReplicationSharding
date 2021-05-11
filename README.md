# ReplicationSharding

This is a simulator to showcase how replication/sharding work behind the scene.
We will use Student management as base of it.
Sample User Data
```
14 Akash 4mn
12 Asheesh srs
2 Ashutosh NTD
1 Bappan NTD
16 Kartik 4mn
8 Mohan su
9 Manan su
3 Mayank NTD
10 Muskan su
13 Shikha srs
5 Suraj f4
6 Sherry f4
4 Umanath NTD
7 Vineet f4
11 Vipin srs
```
## Stage1 | Base Work

### Implementation
* Create a utility via which we can perform the CRUD operation on Student
    - Create : Student data should be stored in file as per the roll number order
    - Retrieve on the basis of roll number: File will be read line by line and then student information would be displayed
    - Update : File will be read line by and then Student record should be updated
    - Delete : File will be read line by line and then Student record should be deleted
* Student metadata
    * Name
    * Roll Number
    * Class
* Utility will take a yaml file as an input to take the detail where student information would be shared

### Problem
What if I delete the file that is storing the student data how we will recover from that?