# Vue 3 Static SPA with Nginx

A decent setup for Vue 3 (SPA) using Nginx. Optimized for performance, security, and low resource usage.

---

## Features

- **Fast static file serving**: Nginx serves pre-built Vue assets with minimal overhead.  
- **SPA routing support**: Handles Vue router history mode with proper fallback to `index.html`.  
- **Production-ready logs**: Access and error logs are directed to Docker-friendly stdout/stderr.  
- **Non-root execution**: Secure configuration compatible with running as a non-root user in Docker.  
- **Optimized for Docker**: Lightweight Alpine-based images with minimal attack surface.  

---

## Use Case

This project is **suited for**:

- Deploying **Vue 3 SPAs** with static assets only.  
- Hosting on **Docker containers**, cloud providers, or simple VM servers.  
- Applications that **do not require server-side rendering** or dynamic backend logic.  
- High-performance static hosting where speed and low resource consumption are critical.

**DO NOT** use it for:

- Where Server-Side Rendering (SSR) is needed.
- Node.js-dependent backend logic inside the same container.
- Apps with dynamic content rendering.
- If you did not LIKE this setup.

---

## Getting Started

### Build the Vue app

```bash
docker compose up -d --build
