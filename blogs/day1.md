# Day 1 of the Cloud Resume Challenge

## **Introduction:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; I've spent my entire professional journey in IT, with a focus on cybersecurity in recent years. Always eager to grow both professionally and personally, I turned to insights from fellow cybersecurity experts online. This led me to discover a captivating "cloud resume challenge," introduced by Forrest Brazeal. I was initially unfamiliar with the concept, but after delving into the details at [Cloud Resume Challenge](https://cloudresumechallenge.dev/docs/the-challenge/aws/), I felt confident in my ability to tackle it. Now, I'm chronicling each step of this endeavor, hoping to refine my expertise further and perhaps inspire some of you to embark on this challenge as well.

### Setting the Stage on the Frontend:

The mission was clear: assemble a cloud-based resume. Luckily, I already had an AWS account, which meant I could dive straight in and make use of the different AWS tools available. My first task? Setting up a static website on Amazon S3.

Making sure I had the correct permissions and access to services like S3, Lambda, and DynamoDB was essential. Then I created a new user specifically for this project, taking extra precautions to adhere to best practices. 

For the frontend of this cloud challenge, I google the interweb for a cool HTML resume template. After exploring a few, I landed on one that perfectly matched my aesthetic. Diving into **Visual Studio Code (VS Code)** was a fresh experience for me, but its integrated terminal was a game-changer. It let me run commands without ever leaving the editor. Plus, by adding the “open with live server” plugin, I could see my changes in real-time, making sure It was looking the way I intended.

### Gitty

With my AWS environment ready, I turned to GitHub to kickstart my repository. After crafting a README that would serve as the backbone of my project's documentation, I was all set for my first commit. But here's where things got tricky.

I ran into an error while trying to push to GitHub: "Support for password authentication was removed." Confused, but only to learn that GitHub had stopped using password authentication for pushing commits smh.

But Instead of throwing in the towel, I found a workaround using a GitHub personal access token. This token acts as an alternative to the traditional password, granting permissions to various GitHub actions. Got my token sorted with the right permissions, plugged it in, and bam! My commit was up and running. 🚀

### **Screenshots as Evidence:**

To provide a visual narrative of my journey, I decided to include screenshots in my GitHub blog. This posed the question: what's the best way to embed images in a GitHub repository?

Enter the GitHub Hack: While the conventional method involves storing images directly within the repository, I came across a cool GitHub hack. When I create a new issue and drag & drop the image into it, GitHub automatically provides a direct URL for the image, even without submitting the issue. This URL can then be used to embed the image in markdown files. A quick and efficient way, especially for temporary or quick visual references!

### **AWS S3 Hosting:**

Once the resume was ready for its online debut, I turned to Amazon S3 for hosting. Setting up an S3 bucket was straightforward, but I faced an blip when trying to access the website. The internets favorite "404 Forbidden" error showed up. With some research and adjustments to the bucket policy, I managed to get the site live.

However, a new challenge arose when trying to link my custom domain. DNS configurations can be tricky, and I was reminded of that when trying to set up a CNAME record for my domain hosted on Squarespace. A conflict with an existing record meant I had to reconfigure my domain setup.

### **Navigating SSL with Amazon CloudFront:**

To make sure my website was secure via HTTPS, I turned to Amazon CloudFront with an SSL certificate from Amazon Certificate Manager (ACM). Here, I encountered a few more challenges:

- The certificate status remained "Pending validation" longer than I expected.
- I opted for DNS validation for the certificate, which required adding a CNAME record to my domain's DNS settings.
- I even had a moment of confusion selecting the correct SSL certificate in CloudFront, as the options were grayed out due to the certificate's pending validation status.

## **Reflecting on Day 1:**

The little bumps in the road reminded me of a few things; just like most things in life, when working in the cloud, things can change quickly, but there’s a solution to everything and being a flexible and knowing when to pivot is part of the journey. 💡

You can find my official cloud resume here 👉🏿:  [Alex's Cloud Resume](https://d29mctvgvn7ma0.cloudfront.net/index.html)

