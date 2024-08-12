# Project - Deploy a Static Website on AWS

The cloud is perfect for hosting static websites that only include HTML, CSS, and JavaScript files that require no server-side processing. The whole project has two major intentions to implement:

Hosting a static website on S3 and Accessing the cached website pages using CloudFront content delivery network (CDN) service as CloudFront offers low latency and high transfer speeds during website rendering.

# The static website files to be uploaded to the S3 bucket include:

- **index.html** - The Index document for the website. 
- **/img** - The background image file for the website. 
- **/vendor** - Bootssrap CSS framework, Font, and JavaScript libraries needed for the website to function. 
- **/css** - CSS files for the website.

- **NOTE:** For **MacOS** users, upload all files in the **"__MACOSX"** folder instead.

# To download the zipped file select it from the file tree, then select "view raw", it should start downloading.
   
# Screenshots of all steps are included in the repository to serve as a guideline for implementing the project.

# Project implementation steps are as follows:

1. Download the zipped "Static Website Files".
2. Create a public S3 bucket.
3. Configure the bucket for website hosting and secure it using IAM policies.
4. Upload the website files to your bucket.  
5. Speed up content delivery using AWS’s content distribution network service, CloudFront.
      - Select “Services” from the top left corner of aws management console and enter “cloudfront” in the “Find a service by name or feature” text box and select “CloudFront”.
      - From the CloudFront dashboard, click “Create Distribution”.
      - Don't select the bucket from the dropdown list. Paste the Static website hosting(bucket) endpoint i.e, <bucket-name>.s3-website-<region>.amazonaws.com.
      - Leave the defaults for the rest of the options, and click “Create Distribution”. It may take up to 10 minutes for the CloudFront Distribution to get created.
      - Once the status of your distribution changes from “In Progress” to “Deployed”, copy the endpoint URL for your CloudFront distribution found in the “Domain Name” column.
7. Then access the website in a browser using the unique CloudFront endpoint/Domain Name

# Topics Covered: 

- AWS - Cloud Computing 
- S3 bucket creation
- S3 bucket configuration to enable static website hosting
- Website distribution via CloudFront
- Access website via web browser
