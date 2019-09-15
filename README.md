# url_shortener_sample

<img src="/src/demo.gif" alt="demo" style="max-width:100%;">

This repository contains all the code examples from the contents as bellow:
[Build a Serverless, Private URL Shortener](https://aws.amazon.com/blogs/compute/build-a-serverless-private-url-shortener/)


# Table of Contents
- Technologies Used
- How to setup
- Notes
- Sources


# Technologies Used
## The followings are used by AWS CloudFormation
- AWS Lambda
- S3 bucket
- API Gateway
- CloudFront


# How to setup
- git clone https://github.com/gkzz/url_shortener_sample.git
- Login AWS console, and select CloudFormation
- Press "Create stack" button 

<img src="/src/url_shortener1.png" alt="how_to_setup1" style="max-width:100%;">

- Change AWS region to that of the appropriate 

- Upload [/url_shortener_sample/rl_shortener.yml](/url_shortener_sample/rl_shortener.yml)

<img src="/src/url_shortener2.png" alt="how_to_setup2" style="max-width:100%;">

- Enter the following parameters:
    - Stack name: "URLShortener"
    - S3BucketName: ${YOUR_UNIQUE_NAME}
    - URLExpiration: 7

<img src="/src/url_shortener3.png" alt="how_to_setup4" style="max-width:100%;">

- Press the check button of "I acknowledge that AWS CloudFormation might create IAM resources"

<img src="/src/url_shortener5.png" alt="how_to_setup5" style="max-width:100%;">

- Status is "CREATE_COMPLETE" on Events page
(It takes 20 to 30 mins to complete it)

<img src="/src/url_shortener_completed.png" alt="completed" style="max-width:100%;">

- Congratulations on the launch of your URL Shortener!
(ConnectURL is that of your service)
<img src="/src/url_shortener_completed2.png" alt="connecturl" style="max-width:100%;">



### Optional
- Enter a monitoring time parameter (e.g. 7)
<img src="/src/url_shortener4.png" alt="how_to_setup4" style="max-width:100%;">

## How to check if your S3BucketName is unique, or not
- Select S3 bucket
- Enter your S3BucketName

<img src="/src/url_shortener_s3.png" alt="s3" style="max-width:100%;">

- If it is not unique, this following error message is displayed:
  "Bucket name must not end with dash or period"

<img src="/src/url_shortener_s3_name.png" alt="check_s3_name" style="max-width:100%;">

# Notes
being prepared.


# Sources
[Build a Serverless, Private URL Shortener](https://aws.amazon.com/blogs/compute/build-a-serverless-private-url-shortener/)
