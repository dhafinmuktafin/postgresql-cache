# postgresql-cache

This is a simple cache implementation using PostgreSQL (instead of redis) with Golang for my learning purposes.

### Table Schema
```
CREATE TABLE IF NOT EXISTS users (
    id SERIAL PRIMARY KEY,
    username VARCHAR(50) UNIQUE NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```
