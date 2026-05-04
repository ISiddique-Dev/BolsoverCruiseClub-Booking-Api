# Bolsover Cruise Club - Booking API (.NET 10)

## Overview
This API serves as a modernized replacement for legacy Access-based booking systems. It demonstrates a **Service-Oriented Architecture** designed for scalability, maintainability, and data integrity.

## Key Modernization Features
* **Transition from Access to SQL:** Utilizes EF Core with LocalDB to provide relational integrity and concurrent user support.
* **Clean Architecture:** Separates Domain Models, Data Access (Repository Pattern), and Business Logic (Service Pattern).
* **Robustness:** Global Exception Handling ensures the API returns standard RFC-7807 error responses instead of stack traces.
* **Validation:** FluentValidation decouples validation logic from the API controllers.

## Tech Stack
* **Framework:** .NET 10 (C#)
* **ORM:** Entity Framework Core
* **Database:** MS SQL Server (LocalDB)
* **Documentation:** Swagger / OpenAPI

## Getting Started
1. Set `FeatureFlags:AddTestData` to `true` in `appsettings.json` to seed initial data.
2. Run `Update-Database` in the Package Manager Console.
3. Launch the project to view Swagger documentation.