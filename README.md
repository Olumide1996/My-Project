# Project Report

### Student Name: Adebisi Olumide 
### Website Link:https://projectmide.xyz 

## Project Task:

Set up a website as part of your Computer Networking project. Your task includes:

1. **Domain & Hosting**: Choose a hosting service and set up a domain (can be free or temporary).
2. **Website Setup**: Create a basic website using HTML, CSS, and optionally JavaScript or a framework of your choice.
3. **Networking Aspects**: Ensure the site is accessible online and demonstrate knowledge of networking concepts such as DNS, IP addresses, and protocols.
4. **Documentation**: Submit a report including your website link, a description of the setup process, challenges faced, and how networking principles were applied.
5. **Bonus**: Implement security features such as HTTPS, firewalls, or access control.

---

## Project Overview:

This project demonstrates the successful setup, security, and documentation of my website project and applies my understanding of both web development and computer networking fundamentals.

---



---

## Setup Process:

### A. Website Setup:
1. Created my project folder (to house all project files).
2. Set up basic files: `index.html`, `styles.css`.
3. Installed **Notepad++** to create my `index.html` website file and structure it.
4. Used **Notepad++** to create my CSS source file for basic website styling.
5. Tested locally by accessing `index.html` in Chrome.

### B. Setting Up Version Control with Git:
1. Initialized a Git repository using the command prompt.
2. Navigated to the project folder and ran the Git initialization command.
3. Added and committed changes to the Git repository.
4. Successfully pushed the changes to a GitHub repository.

### C. Choosing Hosting Service and Deployment:
1. **Deployment using Netlify**: I signed up for a free Netlify account.
2. Connected my Git repository to my Netlify account and selected my active project repository.
3. Deployed the site and received the following URL: [https://olumideadebisiproject.netlify.app/](https://olumideadebisiproject.netlify.app/).

### D. Setting Up a Domain Name:
1. Signed up on a hosting provider (**Namecheap**) and registered the domain: [https://projectmide.xyz/](https://projectmide.xyz/).
2. Configured DNS settings by creating a CName record pointing to my chosen domain.
3. Registered custom DNS nameservers provided by my hosting service.
4. DNS propagation took a few hours to complete.
5. Tested the website using the custom domain in Chrome.
6. Enabled SSL/HTTPS for security, ensuring the site is served securely.

### E. Implementing Networking and Security Aspects:
- The **domain name server** translates human-readable domain names into machine-readable IP addresses, allowing users to access websites without needing to use IP addresses.
- **HTTP/HTTPS protocols**: HTTP is the basic protocol for web traffic, and HTTPS secures the connection using SSL certificates.
- The setup steps were as follows:
  1. The domain name was translated into the IP address using my DNS servers. I confirmed this using the `nslookup` command.
  2. **HTTP/HTTPS Protocols**: Netlify automatically provisions SSL certificates via Let's Encrypt.
  3. **Additional Security**: Netlify provides built-in DDoS protection, firewalls, and OAuth for access control. I implemented OAuth by providing my GitHub client ID and secret key.

---

## Challenges and Lessons Learned:

### Challenges:
1. Deployment errors from GitHub to Netlify, especially around file placement in the `public` folder, which caused "Fatal error" messages.
2. DNS propagation delay of around 1 hour, which delayed the availability of my custom domain.

### Lessons Learned:
1. **DNS and Domain Configuration**: Setting up DNS records and linking them to the domain can be tricky. I learned that DNS propagation can take time, meaning changes might not be reflected immediately, which required patience during testing.
2. **The Importance of HTTPS for Security**: Switching from HTTP to HTTPS is crucial for both security and trustworthiness. HTTPS should be prioritized from the beginning of any web project.
3. **Using Git for Version Control**: Git is essential for managing even smaller projects as it helps organize and safeguard code changes, making it easier to track progress and rollback when needed.

---

## Conclusion:

This project has succesfully tested the knowledge of using both web development technology stack as well as network fundamentals and principles
---
