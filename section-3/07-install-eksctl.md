# eksctl Installation Guide

A step-by-step guide to install eksctl on Linux systems. eksctl is a simple CLI tool for creating and managing Kubernetes clusters on Amazon EKS.

## What is eksctl?

eksctl is the official CLI tool for Amazon EKS (Elastic Kubernetes Service). It simplifies the process of creating, managing, and operating Kubernetes clusters on AWS.

## Prerequisites

- Linux system (Amazon Linux, Ubuntu, etc.)
- Internet connection
- sudo privileges

## Installation Steps

### Step 1: Download the Latest Release

Download the latest eksctl binary directly from GitHub releases:

```bash
curl -LO "https://github.com/eksctl-io/eksctl/releases/latest/download/eksctl_Linux_amd64.tar.gz"
```

This command always downloads the latest stable version. No grep or cut commands required.

### Step 2: Extract the Archive

Extract the downloaded tar.gz file:

```bash
tar -xzf eksctl_Linux_amd64.tar.gz
```

This will extract the `eksctl` binary to your current directory.

### Step 3: Move to System Path

Move the binary to `/usr/local/bin` to make it accessible system-wide:

```bash
sudo mv eksctl /usr/local/bin/
```

### Step 4: Verify Installation

Check that eksctl is installed correctly:

```bash
eksctl version
```

You should see output showing the eksctl version, like:

```
0.XXX.0
```

---

**Installation Complete!** You can now use eksctl to manage your EKS clusters.
