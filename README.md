# WordPress Local Development (Docker)

## Overview

This project provides a complete Docker-based local WordPress development environment using Nginx, MySQL, and phpMyAdmin.

The environment is designed for easy setup, local testing, development, and future reproducibility with documented versions and setup steps.

---

## Features

* WordPress running in Docker containers
* Nginx reverse proxy configuration
* MySQL database integration
* phpMyAdmin database management
* Easy startup and shutdown
* Fully documented setup process

---

## Services and Versions

| Service                   | Version    |
| ------------------------- | ---------- |
| Docker Engine             | 29.5.3     |
| Docker Compose            | v5.1.4     |
| WordPress                 | 6.5.2      |
| PHP (WordPress Container) | 8.2.18     |
| MySQL                     | 8.0.46     |
| Nginx                     | 1.31.2     |
| phpMyAdmin Container      | PHP 8.3.26 |
| Host OS                   | Windows    |

---

## Prerequisites

Install the following before starting:

* Docker Desktop
* Git
* Web Browser (Chrome / Edge)

Verify installation:

```bash
docker --version
docker compose version
```

---

## Clone Repository

```bash
git clone https://github.com/akshagg4242/wordpress-local-development.git
cd wordpress-local-development
```

---

## Project Structure

```text
wordpress-local-development/
│
├── nginx/                 # Nginx configuration
├── src/                   # WordPress source files
├── docker-compose.yml     # Docker services configuration
├── README.md              # Project documentation
└── setup-guide.md         # Setup reference
```

---

## Setup Process

### Step 1 — Start Docker Desktop

Ensure Docker Desktop is installed and running.

---

### Step 2 — Start Containers

Run:

```bash
docker compose up -d
```

This creates and starts:

* WordPress container
* MySQL database container
* Nginx container
* phpMyAdmin container

---

### Step 3 — Verify Running Containers

Run:

```bash
docker compose ps
```

Verify all services are running.

---

### Step 4 — Access the Application

Open:

### WordPress Site

```text
http://localhost
```

### WordPress Admin

```text
http://localhost/wp-admin
```

### phpMyAdmin

```text
http://localhost:8081
```

---

### Step 5 — Configure WordPress

After opening localhost:

1. Select language
2. Configure site details
3. Create admin account
4. Login to Dashboard

---

## Common Commands

### Stop Environment

```bash
docker compose down
```

### Restart Environment

```bash
docker compose restart
```

### View Logs

```bash
docker compose logs
```

### Start Existing Containers

```bash
docker compose start
```

---

## Verification

Environment setup is considered successful when:

* WordPress homepage loads
* Admin dashboard is accessible
* phpMyAdmin opens successfully
* All containers show running status

---

## Screenshots

Project screenshots demonstrating:

* Docker containers
* WordPress homepage
* WordPress dashboard
* phpMyAdmin access

are included in this repository.

---

## Status

Completed, tested, and verified for local development environment setup.
