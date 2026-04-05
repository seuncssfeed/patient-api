# Patient API (.NET 10)

## Overview
This project is a RESTful Web API built using .NET 10 to manage patient records. It was developed as part of a take-home assessment.

## Task 1 Implementation

- Implemented RESTful endpoints for managing patient records:
  - `POST /patients`
  - `GET /patients/{id}`
  - `GET /patients`
  - `PUT /patients/{id}`
- Followed RESTful conventions using resource-based routing
- Used appropriate HTTP status codes:
  - `201 Created` for successful creation
  - `200 OK` for successful retrieval and updates
  - `400 Bad Request` for validation failures
  - `404 Not Found` for missing resources
- Used in-memory storage to persist patient data during runtime
- Implemented OpenAPI documentation using built-in .NET support with Scalar for interactive API exploration
- No authentication was implemented, as specified in the assignment

---

## Task 2 Enhancements

- Implemented request validation for required fields, email format, and guardian requirements for minors
- Standardized validation and not-found error responses using consistent JSON structures
- Added global exception middleware to handle unexpected errors gracefully

---

## Task 3 Enhancements

- Added unit tests using xUnit
- Covered core service methods including patient creation, retrieval, search, and update
- Structured business logic into a dedicated service layer to support testability

---

## How to Run

1. Navigate to the project directory
2. Run:

```bash
dotnet run

