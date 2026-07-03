# Financial Transaction API

A production-inspired financial transactions API built with .NET, PostgreSQL, Redis, Docker and Clean Architecture.

This project simulates core financial operations such as account creation, deposits, withdrawals, transfers and transaction history, applying backend engineering practices commonly used in real-world financial systems.

## Goals

- Build a modern backend API using .NET
- Practice Clean Architecture and Domain-Driven Design principles
- Implement financial transaction rules
- Use PostgreSQL as the main database
- Use Redis for caching and idempotency
- Add automated tests
- Prepare the project for AWS deployment

## Tech Stack

- C#
- .NET 9
- ASP.NET Core
- PostgreSQL
- Redis
- Docker
- Entity Framework Core
- FluentValidation
- MediatR
- Serilog
- xUnit

## Features

- Create account
- Get account details
- Deposit money
- Withdraw money
- Transfer money between accounts
- List account transactions

## Architecture

The solution follows Clean Architecture principles:

- Domain: business entities and rules
- Application: use cases, commands, queries and validations
- Infrastructure: database, cache and external services
- API: HTTP endpoints and application configuration

## Running Locally

```bash
docker compose up -d
dotnet restore
dotnet run --project src/FinancialTransactions.Api