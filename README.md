# AWS Static Website Hosting - End to End Deployment

A static website hosted entirely on AWS using S3, CloudFront, Route 53, ACM, and a GoDaddy custom domain — built manually and deployed using best AWS practices.

---

## Project Structure

aws-static-website-hosting/
├── index.html                       # Main static website file
├── screenshots/                     # Project screenshots
│   ├── s3-bucket.png                # S3 static hosting setup
│   ├── cloudfront.png               # CloudFront distribution
│   ├── route53.png                  # Route 53 hosted zone
│   ├── acm.png                      # SSL certificate validation
│   └── final-website.png            # Final live website
└── README.md                        # Documentation

---

## Overview

This project demonstrates hosting a static website on AWS with a custom domain (aniket123.shop) using:

- S3 → Static website hosting  
- CloudFront → Global CDN + HTTPS  
- ACM (us-east-1) → Free SSL Certificate  
- Route 53 → DNS + Domain Management  
- GoDaddy → Domain registrar  

Live Website: https://aniket123.shop

---

## AWS Setup Workflow

### 1. S3 Static Website
- Created S3 bucket: `20-oct-project-website-hosting`
- Enabled Static Website Hosting
- Uploaded `index.html`
- Made bucket public

### 2. CloudFront Distribution
- Origin: S3 static website endpoint  
- Viewer Protocol Policy: Redirect HTTP → HTTPS  
- Alternate domain names: `aniket123.shop`, `www.aniket123.shop`  
- Custom SSL Certificate (from ACM) attached

### 3. SSL Certificate (ACM)
- Requested in us-east-1 (N. Virginia)
- Added DNS CNAME validation records in Route 53
- Status: Issued

### 4. Route 53 Hosted Zone
- Hosted zone created for `aniket123.shop`
- Records created:
  - A (Alias) → CloudFront distribution  
  - CNAME (www) → CloudFront distribution  
  - CNAME (ACM) → Validation records

### 5. GoDaddy Domain Connection
- Changed GoDaddy nameservers to AWS Route 53 nameservers  
- Waited for propagation  
- Verified DNS resolution via dnschecker.org

---

## Architecture

