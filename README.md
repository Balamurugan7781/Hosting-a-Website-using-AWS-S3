# 🌐 Hosting a Static Website using AWS S3

This project demonstrates how to host a static website using **Amazon Web Services (AWS) S3**. It includes setting up the S3 bucket, configuring permissions, and enabling static website hosting for a simple HTML/CSS-based site.

---

## 🚀 Project Overview

The objective of this project is to gain hands-on experience with AWS services by hosting a static website on Amazon S3. It covers:

- Creating and configuring an S3 bucket
- Uploading website files (HTML, CSS, assets)
- Setting up static website hosting
- Managing bucket policies and permissions for public access
- Testing and verifying website deployment

---


---

## 🛠️ Tools & Technologies Used

- **Amazon S3** – for static website hosting
- **AWS Management Console** – for bucket configuration
- **HTML/CSS** – simple front-end development
- **Bucket Policies** – for public access management
- *(Optional)* Route 53 / CloudFront / ACM – for domain/HTTPS setup *(if applicable)*

---

## 🧭 Steps to Reproduce

1. **Create an S3 Bucket**
   - Bucket name should match the domain name if custom domain is used.
   - Uncheck *Block all public access*.

2. **Enable Static Website Hosting**
   - Specify `index.html` as the index document.
   - (Optional) Add `error.html` as the error document.

3. **Upload Website Files**
   - Upload `index.html`, CSS, and any other assets.

4. **Set Bucket Policy**
   - Add a policy to allow public read access to the files:
     ```json
     {
       "Version": "2012-10-17",
       "Statement": [
         {
           "Sid": "PublicReadGetObject",
           "Effect": "Allow",
           "Principal": "*",
           "Action": "s3:GetObject",
           "Resource": "arn:aws:s3:::your-bucket-name/*"
         }
       ]
     }
     ```

5. **Access the Website**
   - Visit the **S3 static website endpoint URL** provided in the bucket hosting settings.

---

## 📷 Screenshots

*(Optional – include screenshots of the S3 settings, file uploads, and final hosted page for a polished README)*

---

## 🧠 What I Learned

- How to configure AWS S3 for web hosting
- Understanding of public access and bucket policy
- Deploying and testing a static website on the cloud

---

## 📌 Future Enhancements

- Add HTTPS using CloudFront and ACM
- Integrate custom domain via Route 53
- Expand the website to include dynamic content via AWS Lambda/API Gateway

---

## 📬 Contact

Feel free to reach out if you have any questions!

**Author**: Balamurugan  
**Email**: [your-email@example.com]  
**GitHub**: [github.com/Balamurugan7781](https://github.com/Balamurugan7781)

---

