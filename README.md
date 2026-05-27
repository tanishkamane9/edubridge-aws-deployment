# EduBridge - AWS EC2 Website Deployment 🚀

A simple educational landing page website created and deployed on **AWS EC2** to learn cloud deployment and web hosting basics.

This project was built to understand how websites can be hosted on a cloud server using **Amazon EC2**, **Apache Web Server**, and **Linux-based server configuration**.

---

## 🌐 Live Website

**Live Demo:**  
http://65.0.125.160

---

## 📌 About The Project

EduBridge is a basic educational website created for deployment practice.

The main purpose of this project was to learn:

- Hosting a website on AWS EC2
- Connecting to a remote Linux server using SSH
- Configuring Apache Web Server
- Uploading website files to a cloud server
- Deploying HTML, CSS, JavaScript, and image assets

The website includes a responsive landing page with navigation, styled UI components, an image section, and a simple JavaScript interaction.

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript

### Deployment & Cloud
- AWS EC2
- Apache HTTP Server (httpd)
- Amazon Linux 2023
- MobaXterm (SSH & SFTP)

---

## 📂 Project Structure

```text
edubridge/
│── index.html
│── README.md
│
├── css/
│   └── style.css
│
├── js/
│   └── scripts.js
│
└── images/
    └── 1106.jpg
```

---

## ⚙️ Deployment Steps

### 1. Launch EC2 Instance
- Created an EC2 instance on AWS
- Configured Security Group settings
- Enabled HTTP access

### 2. Connect to Server
Connected to EC2 using **MobaXterm SSH** with a `.pem` key.

### 3. Install Apache Web Server

```bash
sudo yum update -y
sudo yum install httpd -y
```

Start Apache:

```bash
sudo systemctl start httpd
sudo systemctl enable httpd
```

### 4. Configure Web Directory

Moved to web root directory:

```bash
cd /var/www/html
```

Created project folders:

```bash
mkdir css js images
```

### 5. Upload Website Files
Uploaded:

- `index.html`
- `css/`
- `js/`
- `images/`

using **MobaXterm SFTP**.

### 6. Deploy Website
Hosted the website publicly using the EC2 public IP.

---

## ✅ Features

- Responsive landing page
- Navigation bar
- Hero section
- Image integration
- CSS styling
- JavaScript button interaction
- Live deployment on AWS

---

## 📚 Learning Outcome

This project helped me understand:

- Basics of AWS EC2
- Linux server navigation
- Apache web hosting
- SSH connection setup
- Website deployment workflow
- Cloud hosting fundamentals

---

## 👩‍💻 Author

**Tanishka Mane**  
Computer Science Engineering Student

GitHub: https://github.com/tanishkaum09
