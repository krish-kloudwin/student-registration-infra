# Student Registration System - Infrastructure

Docker Compose orchestration for the full stack: PostgreSQL, FastAPI backend,
Next.js frontend, and Nginx reverse proxy.

## Sibling repos required
This repo expects `student-registration-backend` and `student-registration-frontend`
to be cloned as SIBLING folders (same parent directory), since docker-compose.yml
builds them via relative paths (`../student-registration-backend`, etc).

## Setup
1. `cp .env.example .env` and fill in real values
2. `htpasswd -bc nginx/.htpasswd yourusername yourpassword`
3. `docker compose up -d --build`
