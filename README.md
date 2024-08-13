# LLM Serve

This project aims to deploy and manage Kubernetes clusters on AWS for serving LLMs using EKS. Below are the steps to install the necessary dependencies.

## Table of Contents

- [How to Install Dependencies](#how-to-install-dependencies)
  - [AWS CLI](#a-aws-cli)
  - [kubectl](#b-kubectl)

## How to Install Dependencies

This section provides instructions on installing the required tools to manage AWS resources and Kubernetes clusters.

### a. AWS CLI

The AWS CLI is a unified tool to manage AWS services from the command line. Follow the steps below to install AWS CLI on macOS using Homebrew.

1. **Update Homebrew:**

   ```bash
   brew update

2. **Install AWS CLI:**

    ```bash
    brew install awscli
   
3. **Verify AWS CLI installation:**

    ```bash
    aws --version
   
### b. kubectl
kubectl is the command-line tool used to interact with Kubernetes clusters. Follow these steps to install it on macOS:

1. **Download the Latest Release:**
Use the following command to download the latest stable version of kubectl:
    ```bash
    curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl"

2. **Make the Binary Executable:**
Modify the file permissions to make the kubectl binary executable:

    ```bash
    chmod +x ./kubectl
   
3. **Move the Binary to a System Path and change ownership:**

    ```bash
    sudo mv ./kubectl /usr/local/bin/kubectl
    sudo chown root: /usr/local/bin/kubectl

To verify the installation, type:

    ```bash
    kubectl version --client --output=yaml





