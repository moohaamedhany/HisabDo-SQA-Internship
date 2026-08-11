# Day 6 – Authentication API Testing (DummyJSON)

## Project Overview

This repository contains my Day 6 submission for the HisabDo SQA Internship Program.

The project focuses on testing Authentication REST APIs using Postman, including positive, negative, boundary, authorization, token, and performance test scenarios.

---

## API Used

https://dummyjson.com

Authentication Endpoints Tested:

- POST /users/add (Registration Simulation)
- POST /auth/login
- GET /auth/me
- POST /auth/refresh
- POST /auth/logout (Behavior Validation)

---

## Tools

- Postman
- DummyJSON REST API
- Microsoft Excel
- GitHub

---

## Test Coverage

### Registration

- Valid Registration
- Missing Required Fields
- Invalid Email
- Empty Request Body
- Duplicate Username

### Login

- Valid Login
- Invalid Password
- Invalid Username
- Empty Username
- Empty Password
- Empty Request
- Token Generation
- Response Validation

### Validation

- Email Format Validation
- Password Boundary Testing
- Missing Password

### Authorization

- Unauthorized Access
- Invalid Token
- Valid Token
- Refresh Token
- Logout Behavior

### Performance

- Login Response Time
- Authenticated Request Response Time

---

## Deliverables

- Postman Collection
- Authentication Test Cases
- Bug Report
- Screenshots
- README

---

## Summary

- Total Test Cases: 30
- Authentication API Tested
- Positive, Negative & Boundary Scenarios
- Token Validation
- Authorization Testing
- Performance Testing

---

## Repository Structure

```
HisabDo-SQA-Day6
│
├── Postman Collection
├── Authentication Test Document.xlsx
├── Screenshots
└── README.md
```

---

## Author

Mohamed Hany

HisabDo SQA Internship – Day 6
