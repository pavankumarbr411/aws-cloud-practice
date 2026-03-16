"Amazon Elastic Compute Cloud (EC2) is a web service that provides scalable virtual servers in the cloud. It is a core component of Amazon Web Services (AWS), enabling users to deploy and manage compute capacity on demand with flexible configurations and pricing models."
# EC2 Instance Creation (AWS Practice)

## Introduction

In this practical exercise, I created a virtual server using **Amazon EC2 (Elastic Compute Cloud)** in **Amazon Web Services (AWS)**. EC2 allows users to run applications on virtual machines in the cloud without managing physical hardware. This practice helped me understand how to launch and configure a basic cloud server using the AWS Management Console.

---

## Step 1: Navigate to the EC2 Service

First, log in to the **AWS Management Console** and search for the **EC2 service**.
EC2 is used to create and manage virtual machines (instances) in the cloud.

Click **Launch Instance** to begin the instance creation process.

---

## Step 2: Configure Instance Name and Operating System

In this step, I configured the basic details of the instance.

* **Instance Name:** `EC2-learner`
  This name helps identify the instance easily in the AWS dashboard, especially when multiple instances are running.

* **Operating System (AMI):**
  I selected **Ubuntu Server 24.04 LTS (HVM), SSD Volume Type**.

### Why this option was selected:

* **Ubuntu** is one of the most widely used Linux distributions for cloud servers.
* **LTS (Long Term Support)** versions are stable and receive long-term security updates.
* **HVM (Hardware Virtual Machine)** provides better performance and compatibility with AWS virtualization.
* **SSD Volume Type** improves storage performance compared to standard storage.

This operating system is commonly used for web servers, backend applications, and cloud development.

---

## Step 3: Create and Select a Key Pair

To securely connect to the EC2 instance, a **Key Pair** is required.

* I created a new key pair named **`mykey`**.

### Why a Key Pair is needed:

* It allows secure authentication when connecting to the instance using **SSH**.
* Instead of using passwords, AWS uses **public-key cryptography** for secure login.
* The `.pem` key file is downloaded and used later to connect to the server from the terminal.

Without a key pair, it is not possible to access the instance securely.

---

## Step 4: Configure Storage

In this step, I used the **default storage configuration**.

### Why the default configuration was selected:

* The default storage size provided by AWS is sufficient for basic practice.
* It falls under the **AWS Free Tier**, which helps avoid extra charges.
* For learning purposes, the default configuration provides enough space for testing and experiments.

---

## Step 5: Launch the Instance

After completing all configurations, I clicked **Launch Instance**.

Once launched successfully, the instance status changed to **Running**, indicating that the virtual server is active and ready to use.

This instance can now be accessed using **SSH** with the previously created key pair.

---

## Result

The EC2 instance **`EC2-learner`** was successfully created and launched using the Ubuntu Server 24.04 LTS operating system. This instance can be used to deploy applications, host websites, or perform further cloud computing experiments.

---

## Key Concepts Learned

* What Amazon EC2 is and how it works
* Selecting an appropriate **AMI (Operating System)**
* Creating and using **Key Pairs for secure access**
* Configuring instance storage
* Launching and managing EC2 instances

This practical exercise helped me understand the basic workflow of creating and launching a cloud server in AWS.
