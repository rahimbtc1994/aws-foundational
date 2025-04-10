# aws-foundational

## 1. Getting Started with Storage

### Intro to storage

#### Benefits
Cost efficient
Secure
Accessible
Scalable
Managed
Backed-up

#### Types : Service
Block : AWS EBS
File  : AWS EFS
Object: AWS S3

#### Choosing the type
1. Define the requirments
2. Select a type
3. Design a strategy

#### Use cases
Block : Hosting db, big data analytics, Entreprise apps
Object : Disaster recovery, data lake, cloud-native apps

## 2. Intro to aws S3
S3 stores objects (ex?) inside bucket, in a specific region

### S3

### Durability and availabality
Durability: is the measure of the average annual expected loss of objects. (aws 99,99999)
Availability: is the amount of time per year that the object is available to users. (99,9)

### Architecture
when upload files to S3 (replicated to min of 3 AZ)

### Backup
Different regions

#### Security
Encryption (3 different algos)
Managment & administration

### Basic workflow
1. moving data to s3
2. s3 accept all type of data
3. one object must be less than 5TO
4. data is stored as object
5. each object has a unique ID
6. object: data, meta-data, key
7. bucket are created in region
8. bucket-name + key + version => unique ID

### Active & Archive

### Classes
Based on the : data access, resiliency, cost

### Cost

## 3. Using AWS S3

### Create a Bucket 
name 
configure the bucket
- choose a region (to minimize latency and cost)
- ownership (based on ACL) + block public acsess
- configure the versioning (disabled by default)
- tags
upload files
copy objects
delete objects

### Lifecycle rules

### Replication rules

### Bucket security

- IAM
- Policies
- Encryption
  
### Migration services

## 4. EFS & EBS

