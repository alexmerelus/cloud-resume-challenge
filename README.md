# My [Cloud Resume](https://www.alexmerelus.me) ☁️

## Introduction
This project is a manifestation of the Cloud Resume Challenge, where I've employed several AWS services and best practices to deploy a static website, integrated with a backend to showcase my resume and cloud skills. With a primary focus on cloud security and compliance templates.

## Features
- **Static Website**: Hosted on AWS S3, presenting my professional journey.
- **Backend API**: Leveraged AWS Lambda and API Gateway to serve dynamic data.
- **Visitor Counter**: Implemented using DynamoDB to track the number of visitors.
- **CI/CD**: Automatic deployment and testing using GitHub Actions.

## Architecture Diagram
![Screenshot 2023-10-11 at 6 36 16 PM](https://github.com/alexmerelus/cloud-resume-challenge/assets/138509128/741de91f-bd8e-4385-ba48-27ca70c83378)

The website "alexmerelus.me" serves as an online resume, displaying visitor counts. It's hosted on Amazon S3 and delivered via CloudFront for speed. The domain is resolved through Amazon Route 53 to CloudFront. The visitor count is fetched via an AJAX request to Amazon API Gateway, which then triggers an AWS Lambda function. This Lambda interacts with DynamoDB to manage the visitor count. Permissions are managed by Amazon IAM, and the system's health is monitored using Amazon CloudWatch.

## Technologies Used
- **AWS Services**: S3 for static hosting, Lambda for serverless computing, API Gateway for routing, DynamoDB for storing visitor counts.
- **Infrastructure as Code (IaC)**: AWS CloudFormation (Coming Soon)
- **CI/CD**: GitHub Actions for automated deployments and testing.


## Challenges and Learning
Venturing into the cloud ecosystem, especially AWS, was a journey filled with challenges. From understanding the intricacies of S3 bucket policies to setting up a serverless backend with Lambda, every step was a learning experience. Emphasizing security and compliance templates deepened my understanding of the importance of cloud security.

## Modifications and Extensions
- **Cloud Security Focus**: Incorporated best practices and templates to ensure the cloud infrastructure is secure and compliant.

## Acknowledgements
Immensely grateful to the Cloud Resume Challenge guidelines and community for valuable resources and insights.

## Contact Information
- **LinkedIn**: [Alex Merelus](https://linkedin.com/in/alexmerelus)
- **Email**: alexmerelus@gmail.com

## License
This project is available under the MIT License.
