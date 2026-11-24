# Risk-assessment
**NAME : Shankar Narayana B**

**REG.NO : 212225220093**

**DATE : 24/11/2026**


**EXPERIMENT 5**

**ASSET-ORIENTED RISK ASSESSMENT OF STORAGE ASSETS IN AWS AND AZURE**

**Objective**

To identify storage assets in AWS S3 and Microsoft Azure Blob Storage, identify possible vulnerabilities and threats, and assess their likelihood, impact, and 
risk level.



**1. Software / Cloud Services Required**

•	AWS Account 

•	Microsoft Azure Account 

•	Web Browser 

•	Internet Connection

Cloud Services Used

Cloud Platform	Storage Service

AWS	Amazon S3

Microsoft Azure	Azure Blob Storage

PART A — AWS S3 STORAGE ASSESSMENT

Step 1: Login to AWS

1.	Open the AWS Management Console. 

2.	Sign in using your AWS account. 

3.	Search for S3. 

4.	Select Amazon S3. 



Step 2: Select the S3 Bucket

1.	Click Buckets. 

2.	Select the S3 bucket created in the previous experiment. 

3.	Record: 

o	Bucket name 

o	AWS Region 

o	Number/type of objects 
<img width="1759" height="894" alt="image" src="https://github.com/user-attachments/assets/940c0d1f-0e21-4222-b03f-074ad49c731f" />





Step 3: Check Block Public Access

1.	Open the S3 bucket. 

2.	Select Permissions. 

3.	Locate Block public access (bucket settings). 

4.	Check Block all public access. 

Record:

•	ON → Secure configuration 

•	OFF → Potential public-access risk 

<img width="1672" height="941" alt="image" src="https://github.com/user-attachments/assets/3d0ace82-e3ef-41c2-bc52-31314c33bdc6" />



Step 4: Check Bucket Versioning

1.	Select the Properties tab. 

2.	Locate Bucket Versioning. 

3.	Record whether it is: 

o	Enabled 

o	Disabled 

Security purpose

Versioning helps recover previous versions of objects after accidental deletion or modification.

<img width="1672" height="941" alt="image" src="https://github.com/user-attachments/assets/d23a2e32-54d9-4e31-82fd-ec90038c8163" />



Step 5: Check Default Encryption

1.	Stay in the Properties tab. 

2.	Locate Default encryption. 

3.	Record the encryption type. 

Possible configurations include:

•	SSE-S3 

•	SSE-KMS 

•	DSSE-KMS 

Security purpose

Encryption protects stored data from unauthorized disclosure.

<img width="1920" height="1200" alt="4" src="https://github.com/user-attachments/assets/39c64738-a8e2-416c-95cd-44664a794c24" />



Step 6: Check Bucket Policy

1.	Select Permissions. 

2.	Locate Bucket policy. 

3.	Check whether a bucket policy exists. 

Record:

•	Policy exists 

•	No policy 

Note

A missing bucket policy is not automatically a vulnerability. Access may be controlled through IAM and other AWS security mechanisms.

<img width="1920" height="1200" alt="5" src="https://github.com/user-attachments/assets/31be1f8f-d528-4eb8-b8db-cd60f22097f3" />


Step 7: Check Object Ownership and ACL

1.	In Permissions, locate Object Ownership. 
2.	Record the current configuration. 

A common secure configuration is:

Bucket owner enforced

This means:

•	ACLs are disabled. 

•	Objects are owned by the bucket owner. 

•	Access is controlled using policies. 

<img width="1920" height="1200" alt="6" src="https://github.com/user-attachments/assets/ccd599f2-8429-48c0-82c7-0c070c114b5a" />


Step 8: Check Server Access Logging

1.	Go to Properties. 

2.	Locate Server access logging. 

3.	Record whether it is: 

o	Enabled 

o	Disabled 

Security purpose

Logging helps investigate suspicious or unauthorized access to the bucket.

<img width="1920" height="1200" alt="7" src="https://github.com/user-attachments/assets/99fb24c9-45bd-4ef2-a636-7d28b150f42d" />

**PART B — AWS RISK ASSESSMENT**

After checking the S3 configuration, identify possible vulnerabilities and threats.

**Risk Formula**

Risk Score = Likelihood × Impact

Use the following scale.

**Likelihood**

<img width="190" height="207" alt="image" src="https://github.com/user-attachments/assets/f04a085e-1253-44bd-8d58-115383ff5917" />

**Sample AWS Risk Assessment**

<img width="822" height="267" alt="image" src="https://github.com/user-attachments/assets/47a1498b-91f9-49fb-84cf-a6a17640ccc9" />

<img width="806" height="312" alt="image" src="https://github.com/user-attachments/assets/c38037f7-66b5-4872-bb60-36289a0836b0" />



**RESULT**

The storage assets in AWS S3 were identified and analyzed. Various security configurations, vulnerabilities, threats, likelihood, and impacts were evaluated. Risk scores were calculated using the Likelihood × Impact method, and appropriate security mitigation measures were recommended.













