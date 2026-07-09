# URL Shortener API

A high-performance URL shortening backend services built with **NestJS**, **TypeScript**, and **TypeORM**. It utilizes **PostgreSQL** as the primary relational database and **Redis** for high-speed caching and URL redirection.

---

## 🚀 Features (Coming Soon / In Progress)
* **URL Shortening:** Generate unique, short codes for long URLs.
* **High-Speed Redirection:** Cached redirects using Redis to maximize performance.
* **Dockerized Infrastructure:** Full development environment ready with a single command.

---

## 🛠️ Prerequisites
Before running this project, make sure you have installed:
* [Node.js](https://nodejs.org/) (v18 or higher)
* [Docker](https://www.docker.com/) & Docker Compose

---

## ⚙️ Project Setup

### 1. Clone the repository
```bash
git clone [https://github.com/UlisesOlmos/url-shortener-api.git](https://github.com/UlisesOlmos/url-shortener-api.git)
cd url-shortener-api
```

### 2. Install dependencies
```bash
npm install
```

### 3. Environment Variables
Copy the example environment file and fill in your local values:
```bash
cp .env.example .env
```

## 🐳 Infrastructure (Docker)
This project uses Docker Compose to manage PostgreSQL and Redis. To spin up the databases in the background, run:

```bash
# Start containers
docker-compose up -d

# Stop containers
docker-compose down

# Stop containers and wipe volumes (reset database)
docker-compose down -v
```

## 👨‍💻 Running the App
Once the Docker containers are healthy and running, you can start the NestJS server:
```bash
# Development mode with hot-reload
npm run start:dev

# Production mode
npm run start:prod
```

## 🧪 Testing
```bash
# Unit tests
npm run test

# End-to-end (e2e) tests
npm run test:e2e
```