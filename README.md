🛡️ Secure-Nexus API Ecosystem
Enterprise-Grade Python Backend with Hybrid REST/GraphQL Architecture

📖 Overview
Secure-Nexus is a high-performance, multi-tenant backend ecosystem designed to demonstrate modern architectural patterns. It bridges the gap between traditional RESTful services and flexible GraphQL data fetching, all while maintaining a "Security-First" posture.

This project was developed using AI-native workflows (Cursor) to ensure 100% test coverage and optimized database query execution.

🏗️ Architectural Highlights
Hybrid API Layer: * FastAPI for high-throughput, latency-sensitive REST endpoints.

Strawberry GraphQL for complex client-side data requirements and reduced over-fetching.

Layered Design: Strict separation between Transport (API), Domain (Service), and Data (Repository) layers.

Asynchronous Processing: Full async/await implementation for non-blocking I/O operations.

🔒 Security & Data Integrity
Auth0/JWT Integration: Implements RS256 asymmetric signing for secure authentication.

Rate Limiting: Sliding-window rate limiting implemented via Redis to prevent DDoS and brute-force attacks.

Pydantic V2 Validation: Advanced data validation and coercion with custom error handlers for "Problem Details" (RFC 7807) compliance.

SQLAlchemy 2.0: Utilizing the 2.0 style API for type-safe database interactions and optimized selectinload for relationship fetching.

🛠️ Performance Tuning & DB Management
Migrations: Managed via Alembic, showcasing complex schema changes and data backfilling scripts.

Indexing Strategy: Explicit use of B-Tree and GIN indexes for optimized search performance on JSONB columns.

Caching: Multi-level caching strategy using Redis for hot-data storage.

🤖 AI-Native Development (Cursor)
This project highlights the use of Cursor and LLMs to accelerate delivery without compromising quality:

Used .cursorrules to enforce PEP 8 and strict type-hinting across the codebase.

AI-assisted refactoring of complex SQL joins into efficient SQLAlchemy models.

Automated generation of edge-case unit tests using pytest and hypothesis.

🚀 Getting Started
Prerequisites
Docker & Docker Compose

Python 3.11+

Poetry (Package Management)

Installation
Clone the repo:

Bash

git clone https://github.com/yourusername/secure-nexus-api.git
Environment Setup:

Bash

cp .env.example .env  # Configure your JWT secrets and DB credentials
Spin up the Ecosystem:

Bash

docker-compose up -d --build
🧪 Testing & Quality Assurance
Run the full suite (Unit, Integration, and Security scans):

Bash

pytest --cov=app --cov-report=term-missing
👨‍💻 Author
Thushan Amarasinghege

Backend Engineer (5+ Years Experience)

PhD Candidate, Laurentian University

LinkedIn Profile
