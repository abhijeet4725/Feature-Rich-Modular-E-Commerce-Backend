# Nexum Backend

> **Feature-Rich Modular E-Commerce Backend**  
> A scalable Spring Boot backend designed for real-world complexity — focused on customers and sellers with AI search, in-app credits, rate limiting, and cloud readiness.

## Key Features

- Role-based access control for CUSTOMER and SELLER
- Secure login via email/phone and Google OAuth 2.0
- Product catalog with browsing, filtering, and sorting
- Full-text smart search with AI-powered voice and image search (planned)
- Cart and checkout with Razorpay payment integration
- Reward-based in-app credits earned and redeemable at checkout (non-transferable)
- Seller dashboard for product and inventory management
- PDF invoice generation and notification hooks (email/SMS)
- Rate limiting and caching using Redis for performance
- Dockerized backend app, PostgreSQL, and Redis for easy local and cloud deployment

## How to Run

### Prerequisites

- Java 21 SDK
- Maven 3.x
- Docker and Docker Compose (for containerized setup)
- PostgreSQL and Redis (can run locally or via Docker Compose)

### Running Locally (Without Docker)

1. Clone the repository  
2. Configure database and Redis settings in `application.yml` or environment variables  
3. Build the project:
```bash
mvn clean package
```

4. Run the application:
```bash
mvn spring-boot:run
```

### Running with Docker Compose

1. Ensure Docker and Docker Compose are installed and running  
2. From the project root directory, run:
```bash
docker compose up --build
```
3. This will build the backend app image (if needed) and start the backend, PostgreSQL, and Redis containers networked together

### Access API Documentation

Swagger UI is available at:  
`http://localhost:8080/swagger-ui.html`

--- 
