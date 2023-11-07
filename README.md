# My [Cloud Resume](https://www.alexmerelus.me) ☁️

## Introduction
This project is a manifestation of the Cloud Resume Challenge, where I'll employ several AWS services and best practices to deploy a static website, integrated with a backend to showcase my resume and cloud skills with projects. With a primary focus on cloud security and compliance templates.
### [AWS IAM Project](https://github.com/alexmerelus/IAM-Cloud-Project)

## Features
- **Static Website**: Hosted on AWS S3, presenting my professional journey.
- **Backend API**: Leveraged AWS Lambda and API Gateway to display votes for projects as they are introduced to the website. 
- **CI/CD**: Automatic deployment and testing using GitHub Actions.

## Architecture Diagram
![Screenshot 2023-10-11 at 6 36 16 PM](https://github.com/alexmerelus/cloud-resume-challenge/assets/138509128/741de91f-bd8e-4385-ba48-27ca70c83378)

The website "alexmerelus.me" serves as an online resume, displaying projects that are combined with a voting system. It's hosted on Amazon S3 and delivered via CloudFront for speed. The domain is resolved through Amazon Route 53 to CloudFront. Utilizing DynamoDB, the vote count is triggered bt the API Gateway, which then triggers an AWS Lambda function. When a visitor clicks the vote button, it makes an API call to the Vote Function to increment the vote. Later, the function will be added to display vote count in real time. Permissions are managed by Amazon IAM, and the system's health is monitored using Amazon CloudWatch.

## Technologies Used
- **AWS Services**: S3 for static hosting, Lambda for serverless computing, API Gateway for routing, DynamoDB for storing project votes.
- **Infrastructure as Code (IaC)**: AWS CloudFormation (Coming Soon)
- **CI/CD**: GitHub Actions for automated deployments and testing.


## Challenges and Learning
In my initial design, I had wanted to add a visitor count to my portfolio. The idea was simple: show a counter that increases every time someone visits the site. It was a way to demonstrate my ability to integrate frontend technologies with cloud-based backend systems. However, during the development process, I encountered challenges related to the CORS (Cross-Origin Resource Sharing) feature.

CORS is essentially a security measure implemented by web browsers to restrict web pages from making requests to a domain different than the one that served the web page. While integrating the visitor count feature, I ran into CORS errors when trying to communicate with my backend service from the frontend. Resolving these CORS issues made the project more complex than I anticipated and beyond my but I still wanted the page to have dynamic elements without being overly complex.

That's when I pivoted to the idea of a "Project Votes" system. Instead of just counting visits, I would let visitors vote on the projects they find most intriguing as they get added to the page. This not only gives me insights into which of my projects resonate most with viewers but also adds an interactive element to my portfolio, enhancing user engagement.

The shift from a passive visitor count to an active voting system also allowed me to delve deeper into cloud technologies and demonstrate more complex integrations. 

## Modifications and Extensions
- **Cloud Security Focus**: Incorporated best practices and templates to ensure the cloud infrastructure is secure and compliant.




## Contact Information
- **LinkedIn**: [Alex Merelus](https://linkedin.com/in/alexmerelus)
- **Email**: alexmerelus@gmail.com
