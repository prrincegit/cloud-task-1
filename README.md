# CLOUD COMPUTING 
**COMPANY**: CODTECH IT SOLUTIONS
**NAME**: PRINCE KUMAR 
**INTERN ID**: CT08DG546
**DOMAIN**:: Cloud Computing
**DURATION**: 8 WEEKS
**MENTOR**: NEELA SANTOSH

# Task 1 - Cloud Storage on AWS S3

## Steps:
1. AWS account created
2. S3 bucket created - Name: `codtech-task1-prince`
3. Example files uploaded
4. Permissions configured
5. Tested with public URL

## Screenshots:
- Bucket List
- Uploaded Files
- File Permission
- Public URL opened

## Why S3?
- Object Storage for unstructured data
- Scalable, Durable
- Easy to share with IAM & Bucket Policies

I implemented a basic cloud storage solution using Amazon S3, which is one of the most popular object storage services in the cloud. I first logged into my AWS account, created a dedicated IAM user with appropriate permissions, and avoided using the root account for daily tasks to follow security best practices.

I created a new S3 bucket and learned about the importance of Block Public Access, which prevents accidental public exposure of data. I uploaded a sample file to the bucket. Initially, I tried making the file public using Access Control Lists (ACLs), but because Bucket Owner Enforced was enabled, the ACL alone did not work — so I applied a Bucket Policy instead. This policy granted public s3:GetObject permission for objects inside the bucket. This taught me the difference between object-level ACLs and bucket-level policies and why policies are the preferred modern method for secure and scalable access control.

I verified that my file was publicly accessible via its Object URL and tested it in the browser. I captured all steps with screenshots and documented them in a README.md file on GitHub, describing how the bucket was created, how public access was configured securely, and how the file can be accessed externally.

This task gave me hands-on experience with creating cloud storage, understanding public vs private access, and applying real-world security controls. If asked in an interview, I can explain why using Bucket Policies over ACLs is a better practice and how to avoid common misconfigurations that could expose data publicly.


