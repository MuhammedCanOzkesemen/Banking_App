# Cashly — Personal Finance & Transaction Management System

## Overview

Cashly is a full-stack personal finance application designed to model real-world financial data handling through a structured backend system.

The project focuses on **transaction processing**, **balance consistency**, and **clean API architecture**, demonstrating how financial operations are validated, persisted, and reflected reliably across the system.

Rather than being a UI-focused project, Cashly emphasizes backend engineering principles such as **separation of concerns**, **data integrity**, and **scalable system design**.

---

## Core Capabilities

* Secure user authentication with hashed credentials (bcrypt)
* Centralized balance management handled on the server
* Income and expense tracking with persistent storage
* Payment processing with automatic balance updates
* Transaction history management with record-level control
* Time-based financial analytics (daily, weekly, monthly, yearly)
* Consistent and structured REST API

---

## Architecture

Cashly follows a layered backend architecture to ensure maintainability and scalability:

* **Controller Layer** — Handles HTTP requests and responses
* **Service Layer** — Contains business logic and validation
* **Model Layer** — Defines database schemas and data structure

### Data Flow

Client → API → Controller → Service → Database → Response → UI

This design ensures that all financial operations are processed centrally and consistently on the server.

---

## Technology Stack

* **Frontend:** HTML5, CSS3, JavaScript (ES6)
* **Backend:** Node.js, Express
* **Database:** MongoDB with Mongoose
* **Security:** bcrypt for password hashing, environment-based configuration
* **Data Processing:** MongoDB aggregation pipelines for analytics

---

## System Design Highlights

* Backend-driven state management (no reliance on frontend state)
* Consistent balance updates across all financial operations
* Modular code structure enabling future scalability
* Clear API contract between frontend and backend
* Structured data models for financial entities

---

## Functional Overview

### Transaction Handling

Users can create income and expense records which are stored in the database and reflected in their financial history.

### Payment Processing

Each payment:

* is validated on the server
* creates a persistent record
* updates the user's balance

### Balance Management

The balance is maintained as a **single source of truth on the backend**, ensuring consistency across all operations.

---

## API Endpoints

### Authentication

* `POST /auth/register`
* `POST /auth/login`

### Transactions

* `POST /transactions`
* `GET /transactions`
* `DELETE /transactions/:id`

### Payments

* `POST /payments`
* `GET /payments`

### Balance

* `GET /balance`
* `PUT /balance` (admin-level operation)

---

## Data Model

### User

Stores identity, authentication credentials, and the current balance.

### Transaction

Represents income and expense entries.

### Payment

Represents outgoing financial operations that affect balance.

---

## Engineering Focus

* Separation of concerns (controller / service / model layers)
* RESTful API design principles
* Consistent financial data handling
* Backend-centric architecture
* Expandable system design for future features

---

## Limitations

* No integration with real banking systems
* No concurrency-safe transaction handling (e.g., race condition protection)
* Basic authentication without advanced session management
* Security is not production-hardened

---

## Planned Improvements

* Fraud detection system (rule-based and ML-based approaches)
* Concurrency-safe transaction processing
* Advanced authentication (refresh tokens, session lifecycle control)
* Enhanced filtering and search for transaction history
* Multi-account and multi-balance support

---

## Summary

Cashly demonstrates how a financial application can be structured from a backend engineering perspective.

It reflects practical understanding of:

* API architecture
* financial data processing
* system design fundamentals

---

## License

MIT
