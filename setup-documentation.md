# WordPress Docker Setup Guide

## Step 1 — Clone Repository

```bash
git clone https://github.com/akshagg4242/wordpress-local-development.git
cd wordpress-local-development
```

---

## Step 2 — Verify Docker

```bash
docker --version
docker compose version
```

---

## Step 3 — Start Containers

```bash
docker compose up -d
```

Verify:

```bash
docker ps
```

---

## Step 4 — Open WordPress

Open browser:

http://localhost

---

## Step 5 — Create WordPress Account

Enter:

- Site Title
- Username
- Password
- Email

Finish installation.

---

## Step 6 — Access Admin Panel

http://localhost/wp-admin

---

## Step 7 — Stop Environment

```bash
docker compose down
```

---

## Troubleshooting

Container logs:

```bash
docker compose logs
```

Restart:

```bash
docker compose restart
```

Remove containers:

```bash
docker compose down -v
```

---

## Status

Environment verified and ready for local development.
