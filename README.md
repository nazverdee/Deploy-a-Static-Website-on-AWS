# AWS Static Website Hosting Project

In this project, a static website was deployed to AWS using multiple core services:

- **Amazon S3** → for static website hosting 

https://my-mini-project-site.s3.us-east-1.amazonaws.com/index.html

- **IAM** → Applying least priviledge.

    - `s3:GetObject`, `s3:PutObject` on `my-bucket` (read/write permissions)
    - Attached policy file: `Admin-policy.json` contains the full policy with the above permissions

- **VPC + EC2** → for hosting a backend server inside a custom network  
- **CloudFront** → for global content delivery and HTTPS support  


<img src="Images/diagram.png" alt="Diagram" width="400">



## Documentation folder 

- Contains extra screenshots