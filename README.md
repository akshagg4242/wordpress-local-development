# WordPress Local Development (Docker)

## Overview
This project provides a Docker-based local WordPress development environment.

## Features
- WordPress + MySQL using Docker
- Nginx configuration
- Local development setup
- Easy startup and teardown

---

## Prerequisites

Install:

- Docker Desktop
- Git

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

## Start Environment

```bash
docker compose up -d
```

---

## Stop Environment

```bash
docker compose down
```

---

## Project Structure

```text
wordpress-local-development/
├── nginx/
├── src/
├── docker-compose.yml
└── README.md
```

---

## Access

WordPress:
```

http://localhost

```

Admin:
```

http://localhost/wp-admin

```

---

## Status

Completed and verified for local development.
