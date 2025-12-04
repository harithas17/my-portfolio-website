# Portfolio Website – AWS S3 + CloudFront + GoDaddy Domain

This repository contains my personal portfolio website and the AWS configuration
used to host it using:

- Amazon S3 (static hosting)
- Amazon CloudFront (CDN + HTTPS)
- GoDaddy (DNS management)

---

## 🚀 Deployment Steps

### 1. Build the project

### 2. Deploy to S3

### 3. Invalidate CloudFront Cache

---

## 🌐 Domain Setup (GoDaddy → CloudFront)

- Added CNAME:  
  Host: www  
  Points to: <my-cloudfront-id>.cloudfront.net  

- Forward to → https://www.harithas.co.uk  
  (Done in GoDaddy Domain Forwarding)

---

## 🔐 Security

- CloudFront OAC is enabled  
- HTTPS enforced  


