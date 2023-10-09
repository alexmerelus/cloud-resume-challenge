# Day 1 of the Cloud Resume Challenge: Embracing Triumphs, Tackling Tribulations

## **Introduction:**

Today marked the beginning of my journey with the Cloud Resume Challenge. As I set forth, my aim was clear: construct a cloud-based resume using AWS services. But as I soon realized, the path was paved with unexpected challenges, learning curves, and, yes, moments of triumph.

## **Frontend Odyssey:**

The day began with the hunt for the perfect minimalistic HTML resume template. After exploring myriad options, I found one that echoed my style. Then came the introduction to Visual Studio Code—a tool unfamiliar to me. Armed with enthusiasm, I delved into customization, ensuring the template reflected my professional journey.

## **Venturing into AWS S3 Hosting:**

With my resume refined and ready, I turned to Amazon S3, anticipating a smooth hosting experience. However, the universe had other plans. Upon trying to access the site, I was met with the formidable "403 Forbidden" error. Not one to be deterred, I researched, reconfigured the bucket policy, and, after some tense moments, celebrated as the site went live.

Yet, the challenges persisted. Linking my custom domain, hosted on Squarespace, to the S3 bucket became a puzzle. DNS configurations, always tricky, necessitated a rethink and reconfiguration of my domain setup.

## **Navigating SSL with Amazon CloudFront:**

A secure website was my next goal, leading me to set up Amazon CloudFront with an SSL certificate via Amazon Certificate Manager (ACM). This stage of the journey was a mixed bag:

- The prolonged wait as my certificate's status remained in "Pending validation".
- The intricate dance of DNS validation, which meant adding a CNAME record to my domain's settings.
- A momentary pause in CloudFront when choosing the SSL certificate, given its pending validation.

## **GitHub: An Unexpected Hurdle**

With the AWS side progressing, I shifted my attention to GitHub, ready to initialize my repository. Crafting a README was my first step—a foundation for my project's documentation. But pushing my initial commit unveiled an unexpected challenge. GitHub had deprecated password authentication, and my commit was denied.

After some research, I stumbled upon a workaround: a GitHub personal access token. This token, when configured correctly, allowed me to bypass the password requirement, and my commit found its way to the repository.

## **Reflecting on Day 1:**

As the day drew to a close, I took a moment to reflect. The unexpected challenges, the triumphs, the moments of doubt, and the subsequent breakthroughs—all made Day 1 an unparalleled learning experience. With the foundation set, I'm now eager to continue my Cloud Resume Challenge journey, ready to face, learn, and share whatever Day 2 brings.

