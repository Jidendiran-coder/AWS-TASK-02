# AWS Task 2: Deploy a Flask Application on an EC2 Instance

## Objective

Deploy a simple Flask app that returns your name when accessed from a browser.

---

## Task Steps

### 1. Launch an EC2 Instance

- **VPC Setup**: Use a custom VPC or the default VPC.
- **Public Subnet**: Place the EC2 instance in a public subnet.
- **Security Group**:
  - **SSH (Port 22)**: Allow access from your IP.
  - **HTTP (Port 80)**: Allow from anywhere (`0.0.0.0/0`).
- **OS**: Choose Ubuntu (e.g., Ubuntu 20.04 LTS).

### 2. Install Flask on EC2 Instance

SSH into the EC2 instance and run the following:

```bash
sudo apt update -y
sudo apt install -y python3 python3-pip
pip3 install flask
