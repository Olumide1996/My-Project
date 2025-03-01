# Computer Networks Project 2


**Website Link:** <https://projectmide.xyz/>
**Student Name:** Adebisi Olumide  

---

## Project Overview
This project demonstrates the successful upgrade of my website, incorporating key security enhancements and performance improvements. The key upgrades include enabling HTTPS, brute-force login attack prevention, page speed optimization, early hints activation, and improved deployment infrastructure using Docker and Kubernetes.

---

## Key Improvements and Justifications
### 1. Enabling HTTPS (SSL Certificate) using Docker containers and Cloudflare
**Why?** To ensure secure data transmission and consistent code reproduction across platforms using Docker.

### 2. Preventing Brute-force Login Attacks using "Under Attack" Mode
**Why?** To enhance website security by requiring users to complete a CAPTCHA before accessing the site.

### 3. Improved Page Speed and User Experience using Cloudflare CDN & Speed Brain
**Why?** Performance optimization through caching and leveraging Cloudflare’s Speculation Rules API.

### 4. Activating Early Hints
**Why?** Allows browsers to preload linked assets, reducing load times and improving user experience.

### 5. Deployment & Infrastructure
- **Deployed as a Docker container in a Kubernetes cluster.**
- **Made accessible publicly using Cloudflare Tunnel.**
- **Why?** To enable Continuous Integration and Continuous Deployment (CI/CD).

---

## Implementation Details

### Part 1: Security Enhancements (Mandatory)

#### 1. HTTP Encryption: Cloudflare Universal SSL
**Steps:**
- Created a Cloudflare account and added the website domain.
- Enabled "Always Use HTTPS" to redirect all HTTP traffic.
- Configured TLS settings to ensure encryption.

#### 2. Brute Force Protection: Cloudflare Rate Limiting
**Steps:**
- Implemented Cloudflare CAPTCHA challenge to show a JavaScript-based challenge upon website visit.

### Part 2: Additional Enhancements

#### 1. Performance Optimization
- **Standard Caching Level:** Configured in Cloudflare to cache static content, improving page load times.
- **Rocket Loader:** Enabled to enhance the loading speed of JavaScript-heavy pages.
- **CDN Configuration:** Cloudflare caching rules set to store static assets (CSS, images) for one week.

#### 2. Network Monitoring and Security Analysis
- Activated Cloudflare Web Analytics for monitoring traffic and security threats.

#### 3. Deployment & Infrastructure
- Migrated website deployment from Netlify to Docker.
- Integrated Docker with Kubernetes for efficient containerized deployment.

### Bonus Challenge: Automated Deployment with Argo CD
- Used **Argo CD** to automate syncing deployments with GitHub and Kubernetes clusters running the website pods.

---

## Challenges & Solutions

### 1. Google reCAPTCHA Errors (Invalid Domain for Site Key)
**Challenge:**
- Persistent errors related to domain mismatches for reCAPTCHA validation.

**Solution:**
- Migrated to Cloudflare's **"Under Attack Mode"** for enhanced security without reCAPTCHA dependency.

### 2. Backend Server Issues with JavaScript
**Challenge:**
- Difficulty in setting up a backend server for the website.

**Solution:**
- Migrated from Netlify to **Docker Hub**, improving integration with **Visual Studio Code**.

### 3. CSS Not Loading in Docker Image
**Challenge:**
- CSS failed to load properly when deployed via Kubernetes.

**Solution:**
- Discovered Kubernetes is case-sensitive; refactored the codebase to comply with Linux-based deployment.

---

## Screenshots of Implemented Features
1. **Brute Force Prevention Using Under Attack Mode**:
![Brute Force Prevention Using Under Attack Mode](https://github.com/Olumide1996/My-Project/raw/main/img/under_attack.jpg)
2. **Website Interface Preview**:
![Website Interface Preview](https://github.com/Olumide1996/My-Project/raw/main/img/web_interface.png)