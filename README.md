# Credit Approval Backend System

A Django REST Framework–based backend service that simulates a lending infrastructure workflow for evaluating borrower eligibility and processing loan approval decisions using structured PostgreSQL data models.

This project demonstrates how financial platforms can automate credit scoring, eligibility checks, and loan lifecycle tracking through scalable REST APIs.

---

## Features

- Customer registration service
- Credit eligibility evaluation engine
- Loan approval decision workflow
- Loan history tracking per customer
- REST API endpoints for lending infrastructure simulation
- Docker-based containerized setup
- PostgreSQL-backed relational data storage

---

## Tech Stack

- Python
- Django
- Django REST Framework
- PostgreSQL
- Docker
- Docker Compose

---

## API Endpoints

All endpoints are available under:

/api/v1/

### Available APIs

POST /register/
Create a new customer profile

POST /check-eligibility/
Evaluate borrower eligibility using credit score logic

POST /create-loan/
Process a loan application after eligibility validation

GET /view-loan/<loan_id>/
Retrieve loan details by loan ID

GET /view-loans/<customer_id>/
Retrieve all loans linked to a customer

---

## Project Architecture Highlights

This backend system demonstrates:

- relational schema modeling for lending workflows
- modular Django app structure
- REST API design for financial decision pipelines
- eligibility computation logic
- containerized deployment environment

These components reflect how lending infrastructure services operate internally in fintech platforms.

---

## Running the Project Locally

Clone repository

git clone https://github.com/Pranjalmishr1/credit-approval-backend.git

Navigate into project directory

cd credit-approval-backend

Start Docker services

docker-compose up

Access API

http://localhost:8000/api/v1/

---

## Environment Setup

Create a `.env` file in project root and add:

SECRET_KEY=your_secret_key_here

Generate a key using:

from django.core.management.utils import get_random_secret_key
get_random_secret_key()

---

## Use Case

This project simulates backend infrastructure used in lending platforms to:

- evaluate borrower eligibility
- process structured approval decisions
- manage loan lifecycle data
- expose APIs consumed by external financial services

---

## Author

**Pranjal Mishra**

Backend Developer | Django | PostgreSQL | REST APIs | Fintech Systems

LinkedIn:
https://www.linkedin.com/in/1pranjal-mishra

GitHub:
https://github.com/Pranjalmishr1