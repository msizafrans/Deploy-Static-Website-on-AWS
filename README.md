# Project - Deploy a Static Website on AWS

The cloud is perfect for hosting static websites that only include HTML, CSS, and JavaScript files that require no server-side processing. The whole project has two major intentions to implement:

Hosting a static website on S3 and Accessing the cached website pages using CloudFront content delivery network (CDN) service as CloudFront offers low latency and high transfer speeds during website rendering.

# Working files uploaded to the S3 bucket includes:

index.html - The Index document for the website. 
/img - The background image file for the website. 
/vendor - Bootssrap CSS framework, Font, and JavaScript libraries needed for the website to function. 
/css - CSS files for the website.

# Project implementation steps are as follows:

1. Download the zipped website files
2. Create a public S3 bucket and upload the website files to your bucket. 
3. Configure the bucket for website hosting and secure it using IAM policies. 
4. Speed up content delivery using AWS’s content distribution network service, CloudFront. 
5. Then access the website in a browser using the unique CloudFront endpoint.

# Topics Covered: 

S3 bucket creation,
S3 bucket configuration,
Website distribution via CloudFront and
Access website via web browser
