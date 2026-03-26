# AWS EC2 Nginx Deployment

## Project Objective

The objective of this project is to launch an AWS EC2 instance, install Nginx, and host a simple webpage that is accessible over the internet.

## Step 1: Launch EC2 Instance

* Go to AWS Console and open EC2 service
* Launch a new instance
* Select Ubuntu Server 24.04 LTS
* Create or select a key pair
* Configure Security Group to allow HTTP (port 80)
* Launch the instance

## Step 2: Connect to EC2 Instance

```bash
ssh -i your-key.pem ubuntu@<public-ip>
```

Switch to root user:

```bash
sudo -i
```

## Step 3: Install Nginx

Update system packages:

```bash
apt-get update
```

Install Nginx:

```bash
apt-get install nginx -y
```

## Step 4: Verify Nginx Installation

Check configuration:

```bash
nginx -t
```

Check Nginx status:

```bash
systemctl status nginx
```

Test locally:

```bash
curl localhost
```

## Step 5: Navigate to Web Directory

```bash
cd /var/www/html
```

List files:

```bash
ls -l
```

Default file present:
index.nginx-debian.html

## Step 6: Create Custom Web Page

```bash
echo "Welcome to Nginx Service" > index.html
```

## Step 7: Verify Output

```bash
curl localhost
```

Expected output:
Welcome to Nginx Service

## Step 8: Access from Browser

Open the following in your browser:
http://<your-ec2-public-ip>

## Troubleshooting

If the site is not accessible:

* Check Security Group and allow HTTP (port 80)
* Ensure Nginx is running:

```bash
systemctl restart nginx
```

## Key Learnings

* AWS EC2 instance setup
* Linux command usage
* Nginx installation and configuration
* Networking concepts such as ports and security groups
* Hosting a webpage on a cloud server

## Conclusion

Successfully deployed a web server on AWS EC2 using Nginx and hosted a webpage accessible via public IP.
