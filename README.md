# AWS Static Website Hosting – End-to-End Deployment

This project demonstrates a complete AWS-based setup for hosting a static website with a custom domain and HTTPS.  
It’s designed, implemented, and optimized using AWS best practices — focusing on scalability, cost efficiency, and security.

---

## Overview

As part of my cloud implementation work, I designed a fully managed solution using **Amazon S3**, **CloudFront**, **Route 53**, and **AWS Certificate Manager (ACM)**.  
The domain was purchased from **GoDaddy** and integrated with Route 53 for DNS management.

The goal was to deliver a static website with:
- Secure HTTPS access  
- Global content delivery through CloudFront  
- Custom domain setup (`aniket123.shop`)  
- Serverless and low-cost architecture  

This approach is similar to what I’ve deployed in production for internal applications and client-facing static sites.

---

## Architecture
End User → Route 53 (DNS)
→ CloudFront (CDN + HTTPS)
→ AWS ACM (SSL/TLS Certificate)
→ S3 (Static Website Hosting)
← GoDaddy (Domain Registrar)


**Services Used:**
- **Amazon S3** – Static website hosting  
- **Amazon CloudFront** – CDN and SSL termination  
- **AWS ACM** – Managed SSL/TLS certificate  
- **Amazon Route 53** – DNS and domain mapping  
- **GoDaddy** – Domain registration and delegation  

---

## Key Highlights

- Designed an **end-to-end AWS static website setup** using only managed services  
- Configured **CloudFront** for HTTPS, caching, and custom domains  
- Implemented **ACM SSL certificate** (DNS validated in us-east-1)  
- Managed **Route 53 hosted zones** and domain delegation from GoDaddy  
- Ensured complete cost transparency — entire setup runs under **$1/month**  
- Followed **AWS Well-Architected Framework** principles (cost, performance, security)

---

## Folder Structure
aws-static-website-hosting/
├── index.html # Main static website file (hosted on S3)
├── README.md # Project overview and details
│
├── Architecture/ # Folder containing architecture visuals
│ └── Architecture.png.png # AWS architecture diagram
│
├── Documentation/ # Folder containing project report
│ └── Project Documentation.pdf # Detailed documentation file
│
├── screenshots/ # AWS service configuration screenshots
│ ├── s3-bucket-1.png # S3 static hosting setup
│ ├── cloudfront2.png # CloudFront distribution details
│ ├── route53-3.png # Route 53 hosted zone and DNS records
│ ├── acm-4.png # SSL certificate (ACM) validation
│ └── final-website-5.png # Final hosted website output



---

### 📘 Folder Details

| Folder | Description |
|---------|--------------|
| **Architecture/** | Contains the AWS static website architecture diagram (PNG format). |
| **Documentation/** | Stores the detailed project documentation in PDF format. |
| **screenshots/** | Includes screenshots from AWS Console (S3, CloudFront, Route 53, ACM, and final website). |
| **index.html** | The main static web page file hosted on S3. |
| **README.md** | Overview and technical explanation of the entire project. |

---

### 💡 Notes
- The naming convention is kept simple and clear for better GitHub readability.  
- Folder names start with a capital letter (for Architecture, Documentation) — this is good practice for professional repos.  
- Screenshots are numbered and labeled to reflect the exact AWS setup order (S3 → CloudFront → Route53 → ACM → Final Website).  

---

✅ This version matches your **current GitHub repo exactly** — no renaming needed, no confusion.

Would you like me to now give you the **short README.md content** for each folder (`Architecture/`, `Documentation/`, and `screenshots/`) — so each folder has its own mini-description file inside (it looks super professional to recruiters)?


## Author

**Name:** Aniket Talwekar  
**Experience:** 3+ years in AWS Cloud & DevOps  
**Role:** Cloud Engineer  
**Expertise:** AWS | Terraform | Jenkins | Docker | AWS EKS/ECR | CI/CD | Infrastructure Automation  

**GitHub:** []
**LinkedIn:** []



