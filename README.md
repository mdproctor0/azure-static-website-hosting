<img width="1536" height="1024" alt="ChatGPT Image Mar 10, 2026 at 02_55_37 PM" src="https://github.com/user-attachments/assets/a41271a4-0c09-4b44-aa83-e11be0dedf11" />

# Azure Static Website Hosting Project

This project demonstrates how to deploy a publicly accessible static website using **Azure Storage Static Website hosting**. The deployment showcases foundational cloud engineering concepts including **object storage, resource organization, and cloud-based web hosting**.

The website is hosted directly from **Azure Blob Storage** without requiring traditional web servers.

<img width="1293" height="468" alt="Screenshot 2026-03-10 at 2 49 36 PM" src="https://github.com/user-attachments/assets/1bfb7806-663f-4827-b824-38d5cda22602" />

---

# Live Website

https://proctorcloud.z13.web.core.windows.net/

---

# Architecture Overview

```
User
 │
 │
Azure Storage Static Website
 │
 │
$web container
 │
 ├── index.html
 └── styles.css
```

This architecture demonstrates how static website assets can be served directly from **Azure object storage**.

---

# Azure Services Used

- Azure Resource Groups
- Azure Storage Account
- Azure Blob Storage
- Azure Static Website Hosting

---

# Project Structure

```
azure-static-website-hosting

README.md

website/
   index.html
   styles.css

screenshots/
   resource-group.png
   storage-account.png
   static-website-enabled.png
   website-live.png
```

---

# Deployment Walkthrough

## 1. Create Resource Group

A dedicated **Azure Resource Group** was created to logically organize all cloud resources used in the project.

![Resource Group](screenshots/resource-group.png)

---

## 2. Deploy Azure Storage Account

An **Azure Storage Account** was deployed to host the static website files using **Blob Storage**.

![Storage Account](screenshots/storage-account-created.png)

---

## 3. Enable Static Website Hosting

Static Website hosting was enabled within the Storage Account.  
This automatically created the **$web container**, which stores the website files.

![Static Website Enabled](screenshots/static-website-enabled.png)

---

## 4. Upload Website Files

The website files were uploaded to the **$web container**.

```
index.html
styles.css
```

---

## 5. Validate Live Deployment

The static website was successfully deployed and made publicly accessible through the Azure storage endpoint.

![Live Website](screenshots/website-live.png)

---

# Key Cloud Concepts Demonstrated

- Object storage for web hosting
- Static website deployment without traditional servers
- Cloud resource organization with Resource Groups
- Blob container architecture
- Cloud application deployment workflow

---

# Skills Demonstrated

Azure, Cloud Architecture, Azure Storage, Blob Storage, Static Website Hosting, Resource Groups, HTML, CSS

---

# Future Improvements

Possible enhancements to this project include:

- Configure **Azure CDN for global caching**
- Add **custom domain name**
- Deploy infrastructure using **Terraform**
- Implement **monitoring and logging**

---

# Author

**Marquell Proctor**

Cloud Engineering Portfolio Project
