# 🚀 Blog Generation API on AWS (Serverless + Bedrock)

A serverless Generative AI API that generates 200-word blog posts using **Amazon Bedrock (Llama 3)** and stores the output in **Amazon S3**.

---

## 🏗 Architecture

<img width="1108" height="624" alt="AWS Architecture Diagram" src="https://github.com/user-attachments/assets/d3df9e0c-3cc0-442e-a57d-84f8a598178e" />

---

## 🛠 Tech Stack

- AWS Lambda (Python)
- Amazon API Gateway
- Amazon Bedrock (`meta.llama3-8b-instruct-v1:0`)
- Amazon S3
- IAM
- CloudWatch
- boto3

---

## 📥 Request Format

```json
{
  "blog_topic": "Generative AI in Healthcare"
}
📤 Output

Generated blog is saved to:

s3://awsbedrockmaaz/blog-output/<timestamp>.txt
🔐 Required IAM Permissions

bedrock:InvokeModel

s3:PutObject

CloudWatch logging permissions

📦 requirements.txt
boto3
botocore
🌎 Region

ca-central-1
