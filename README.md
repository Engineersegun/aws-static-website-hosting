# 🚀 AWS Static Website Hosting
Serverless web hosting on AWS using S3,Route 53,and CloudFront
<img width="1366" height="768" alt="Screenshot (115)" src="https://github.com/user-attachments/assets/37ddd921-a914-415c-a8fe-5beb6b01f3a4" />
<img width="1366" height="768" alt="Screenshot (109)" src="https://github.com/user-attachments/assets/eefae6d1-c52e-4423-b0c5-7e9a7ea1132e" />

### 🏗️ Architecture Explained
The diagram above illustrates the request flow of the application:
* **User Request:** The user enters the domain name managed by **Route 53**.
* **Content Delivery:** **Amazon CloudFront** acts as a CDN, fetching content from the origin and caching it at edge locations for lower latency.
* **Storage:** The static files (HTML/CSS) are securely stored in an **Amazon S3** bucket.
* **Security:** Access is restricted via **S3 Bucket Policies**, ensuring only the CDN can retrieve the files.

### 🚀 Key Technical Features
* **High Availability:** Distributed across multiple AWS Availability Zones.
* **Scalability:** Serverless design that handles traffic spikes without manual intervention.
* **Security:** Implements HTTPS via SSL/TLS certificates and restricted IAM policies.
* **Cost-Efficiency:** Pay-as-you-go model with zero cost for idle time.
