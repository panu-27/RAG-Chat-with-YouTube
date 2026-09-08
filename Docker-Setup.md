# 🐳 Docker Setup Guide

This document covers how to run this application using Docker for both development and production-like environments.

## Before You Begin

Let's make sure you have everything you need:

- **Docker Desktop**: Ensure Docker is installed and running on your system. [Install Docker Desktop](https://www.docker.com/products/docker-desktop/).
- **Environment File**: Create a `.env` file in the project root with your configuration variables. Reference the `_env_template.txt` file for required variables.


---

## 👩💻 For Developers

Ready to hack on the code? This section is for you! We'll set up a development environment with **auto-reload**, so your changes appear instantly.

Simply run:
```bash
docker compose up -d
```

**Key development features:**
- Volume mounting for live code synchronization
- Any code changes you make will automatically trigger a reload
- No manual image rebuilding required

To stop everything, just press Ctrl+C

---

## 🚀 For local deployment
Just want to run the application? Perfect! This command will pull the pre-built images and start everything for you.
```bash
docker compose -f docker-compose.yml up -d
```
**Need Help?**
If you run into any issues:
- Make sure Docker Desktop is running
- Verify your .env file is properly configured
- Check that no other services are using the same ports


Welcome aboard! 🎉