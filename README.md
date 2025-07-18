## Cloud-Vault

Cloud-Vault is a robust, serverless cloud storage solution built on AWS S3, designed to provide secure and efficient file and folder management. It features seamless Google OAuth 2.0 authentication, integrated Razorpay subscriptions, and a scalable backend powered by AWS Lambda and PostgreSQL.

## 🚀 Features

Folder Management: Effortlessly create, rename, and delete folders to organize your files.

File Uploads: Securely upload files of any type directly to AWS S3.

Google Authentication: Secure user authentication powered by Google OAuth 2.0.

Subscription System: Integrated Razorpay for managing user subscriptions and payments.

Serverless Architecture: Highly scalable and cost-effective backend built with AWS Lambda and the Serverless Framework.

Data Management: Efficient data handling with PostgreSQL and Prisma ORM.

Monorepo Structure: Streamlined development and dependency management using Yarn workspaces.

## 🛠️ Tech Stack

| Feature            | Technology                            |
|--------------------|---------------------------------------|
| **Backend**        | AWS Lambda (Serverless Framework)     |
| **Cloud Storage**  | AWS S3                                |
| **Payment Gateway**| Razorpay                              |
| **Authentication** | Google OAuth 2.0                     |
| **Database**       | PostgreSQL                            |
| **ORM**            | Prisma                                |
| **Package Manager**| Yarn (Monorepo)                       |
| **Hosting**        | AWS                                   |


## 📋 Prerequisites

Before you begin, ensure you have the following installed and configured:

Node.js: v14 or higher recommended.

Yarn: Installed globally (npm install -g yarn).

AWS CLI: Configured with appropriate IAM permissions for S3, Lambda, etc.

Razorpay Account: With API Key ID and Secret.

Google Cloud Project: With OAuth 2.0 credentials (Client ID and Client Secret).

PostgreSQL: An instance running locally or accessible remotely.

Serverless Framework: Installed globally (npm install -g serverless).

## ⚙️ Installation

Follow these steps to get your Cloud-Vault project up and running:

1️⃣ Clone the repository
git clone https://github.com/bansalmohit123/cloud-vault.git
cd cloud-vault

2️⃣ Install dependencies
yarn install

3️⃣ Set up environment variables
Create a .env file in the root directory and populate it with your credentials:

# AWS Configuration
AWS_ACCESS_KEY_ID=your-aws-access-key-id

AWS_SECRET_ACCESS_KEY=your-aws-secret-access-key

AWS_REGION=your-aws-region

S3_BUCKET_NAME=your-s3-bucket-name

# Google OAuth Configuration
AUTH_GOOGLE_ID=your-google-client-id

AUTH_GOOGLE_SECRET=your-google-client-secret

AUTH_SECRET=your-auth-secret

# Database Configuration
DATABASE_URL="postgresql://username:password@host:port/database-name"

# Razorpay Configuration
RAZORPAY_KEY_ID=your-razorpay-key-id

RAZORPAY_KEY_SECRET=your-razorpay-key-secret

NEXT_PUBLIC_RAZORPAY_KEY_ID=your-razorpay-key-id

# Server Configuration
SERVER_URL=your-server-url

## 🚀 Running the Project

Development
To run the project locally using the Serverless Offline plugin:

yarn dev

Your server will typically be accessible at:
http://localhost:3000

## 🌐 Deployment

To deploy your Cloud-Vault project to AWS:

yarn deploy

Upon successful deployment, the Serverless Framework will provide the endpoint URLs for your deployed services.

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.
