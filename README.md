# Automating Podman and GHCR with GitHub Actions

This repository demonstrates how to automate container image builds and deployments using **Podman** and **GitHub Container Registry (GHCR)** with **GitHub Actions**. It provides a ready-to-use GitHub Actions workflow to streamline your CI/CD pipeline for containerized applications.

---

## Features
- **Automated CI/CD Pipeline**: Build and push container images to GHCR on every push to the `main` branch.
- **Podman Integration**: Use Podman's daemonless architecture for lightweight and secure container builds.
- **GitHub Actions Workflow**: A sample workflow file (`.github/workflows/podman-ghcr.yml`) is included for easy setup.
- **Secure Authentication**: Uses GitHub's `GITHUB_TOKEN` for seamless authentication with GHCR.

---

## Workflow Overview
The included workflow automates the following steps:
1. **Checkout the code**: Pulls the latest code from the repository.
2. **Set up Podman**: Configures Podman to authenticate with GHCR.
3. **Build the container image**: Uses Podman to build the image.
4. **Push the image to GHCR**: Uploads the built image to GitHub Container Registry.
5. **Verify the image**: Optionally lists the images to verify the build.

---

## Getting Started
1. **Fork or Clone this Repository**:
   ```bash
   git clone https://github.com/byteshiva/podman-ghcr-automation.git
   cd podman-ghcr-automation
