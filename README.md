# Portfolio Website – AWS S3 + CloudFront + GoDaddy Domain

This repository contains my personal portfolio website and the AWS configuration
used to host it using:

- Amazon S3 (static hosting)
- Amazon CloudFront (CDN + HTTPS)
- GoDaddy (DNS management)

---

## 📁 Repository Structure

src/                # Original editable template  
dist/               # Built static files uploaded to S3  
infrastructure/     # AWS configs + GoDaddy DNS instructions  
scripts/            # Build & deploy automation  

---

## 🚀 Deployment Steps

### 1. Build the project
bash scripts/build.sh

### 2. Deploy to S3
bash scripts/deploy.sh

### 3. Invalidate CloudFront Cache
bash scripts/invalidate.sh

---

## 🌐 Domain Setup (GoDaddy → CloudFront)

- Add CNAME:  
  Host: www  
  Points to: <your-cloudfront-id>.cloudfront.net  

- Forward example.com → https://www.example.com  
  (Done in GoDaddy Domain Forwarding)

- SSL via AWS Certificate Manager (Region: us-east-1)

---

## 🔐 Security

- S3 bucket is private  
- CloudFront OAC is enabled  
- HTTPS enforced  

---

## 📝 License
MIT
