## AWS S3 Static Website Hosting Using CloudFormation

## Project Overview

In this project, I deployed a static website using Amazon S3, AWS CloudFormation, and the AWS Command Line Interface (CLI).

The objective was to gain practical experience with Infrastructure as Code (IaC), automated resource provisioning, S3 static website hosting, and AWS access permissions.

I created a CloudFormation YAML template to provision an S3 bucket and configured it to host a simple HTML website.

During deployment, I encountered an AccessDenied error when attempting to access the website. I investigated the S3 bucket’s public access settings and updated the CloudFormation template to configure the required permissions.

After resolving the access issue, I successfully accessed the website through the browser and verified that the HTML content was being served from Amazon S3.

Once testing was complete, I removed the uploaded website files and deleted the CloudFormation stack to clean up the AWS resources.

## AWS Services Used

* Amazon S3: Used to store and host the static HTML website.
* AWS CloudFormation: Used to provision and manage the S3 bucket and its configuration through a YAML template.
* AWS CLI: Used to deploy and update the CloudFormation stack, upload the HTML file, verify deployment status, and remove resources.
* AWS IAM: Provided the permissions required to manage AWS resources through the CLI.

## Project Configuration

* AWS Region: eu-west-2 (London)
* S3 Bucket: my-static-website-ds
* CloudFormation Stack: s3-web-stack
* Website File: index.html
* Infrastructure Template: s3-static.yaml
* Website Hosting: Amazon S3 static website hosting
* Access Configuration: S3 bucket policy permitting public read access to website objects
