# Basic Microservices Docker Setup

## How to run

1. Clone this repository:

```bash
git clone <tvoj-repo-url>
cd <tvoj-repo-folder>
```

2. Build and start all services using docker-compose:

```bash
docker-compose up --build
```

3. After containers start:

- Spring Boot app will be available on [http://localhost:8080](http://localhost:8080)
- Node app will be available on [http://localhost:3000](http://localhost:3000)

4. Verify the setup:

Run the health check script locally:

```bash
bash <(curl -s https://raw.githubusercontent.com/kkenan/basic-microservices/master/health_check.sh)
```

You should see:

```
All checks passed. Congrats!
```

---

## Notes

- PostgreSQL runs on port 5432 with user `demo`, password `demo`, and database `demo`.
- Make sure Docker and Docker Compose are installed on your system.
