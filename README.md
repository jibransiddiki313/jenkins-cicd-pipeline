# Jenkins CI/CD Pipeline 🚀

## Overview
End-to-end CI/CD pipeline built using Jenkins, Docker, and AWS EC2.
Automatically builds and deploys on every code push.

## Architecture
GitHub Push → Webhook → Jenkins → Docker Build → Deploy on AWS EC2

## Pipeline Stages
- Code → Clones latest code from GitHub
- Build → Builds Docker image
- Test → Runs application tests
- Deploy → Deploys using Docker Compose

## Tech Stack
- CI/CD: Jenkins
- Containerization: Docker, Docker Compose
- Cloud: AWS EC2 (Ubuntu 22.04)
- Version Control: GitHub + Webhooks
- OS: Linux (Ubuntu)

## What I Learned
- Jenkins Freestyle and Pipeline Jobs
- GitHub Webhook auto-trigger setup
- Docker Compose deployment
- Debugging Jenkins 403 webhook error
- AWS EC2 disk space management using EBS resize

## How to Run
1. Clone this repo
2. Setup Jenkins on Ubuntu
3. Add GitHub Webhook
4. Run pipeline and app auto deploys
