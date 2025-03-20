# Docker Image Security Scan with Trivy in GitHub Actions

## Overview

This repository contains a GitHub Actions workflow to automatically scan Docker images for vulnerabilities using Trivy.You can easily replace the Docker image name in the workflow to scan your own images.

## Prerequisites

- Docker image hosted on Docker Hub or any other container registry.
- A GitHub repository
- GitHub Actions enabled in your repository.

## Steps Guide

1. Clone this repository to your local machine.

       git clone <repo_url>
       cd <repo_directory>

2. Replace the Docker Image Name:

        docker pull <YOUR_DOCKER_IMAGE>:<TAG>
        trivy image <YOUR_DOCKER_IMAGE>:<TAG>


3. Commit and Push:

          git add .
          git commit -m "Add trivy scan workflow"
          git push origin <branch name>

4. View the Scan Results:

- Go to the Actions tab in your repository.
- Select the latest workflow run.
- Review the vulnerability report
