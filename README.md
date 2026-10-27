# aws-ec2-nginx-dashboard
Multi-page dashboard hosted on AWS EC2 using Nginx
## Preview
[Dashboard]
Dashboard.png
Nginx-Status.png
Report dashboard.png
User dashboard.png

## Features
- Sidebar navigation (Dashboard, Users, Reports, Settings)
- Stat cards and tabbed content
- Responsive layout

## Tech Stack
- HTML, CSS, JavaScript
- Nginx
- AWS EC2 (Ubuntu, t3.micro, Mumbai region)

## Deployment Steps
1. Launch an Ubuntu EC2 instance and create a key pair
2. Allow HTTP (port 80) and SSH (port 22) in the security group
3. Connect to the instance and install Nginx:
   sudo apt update
   sudo apt install nginx -y
4. Start and enable Nginx:
   sudo systemctl start nginx
   sudo systemctl enable nginx
5. Copy the code to the web root:
   sudo nano /var/www/html/index.html
6. Open http://<your-public-ip> in the browser

## What I Learned
- How EC2, security groups, and key pairs work together
- How Nginx serves static files
  

## Future Improvements
- HTTPS with Let's Encrypt
- Custom domain with Route 53
- CI/CD with GitHub Actions
