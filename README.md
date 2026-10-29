# User Management API Testing

## Project Overview

This project demonstrates API testing using **Postman**. It covers basic CRUD operations and negative test scenarios for a User Management API.

The collection contains five API requests to verify response status codes and validate API behavior.

## Tools Used

- **Postman** – API testing and request execution
- **REST API** – HTTP methods and endpoint testing
- **GitHub** – Version control and project documentation

## Test Scenarios

| Test Case | HTTP Method | Endpoint | Expected Status Code |
|---|---|---|---|
| Get all users | GET | `/users` | 200 OK |
| Get one user | GET | `/users/1` | 200 OK |
| Create a user | POST | `/users` | 201 Created |
| Get nonexistent user | GET | `/users/999` | 404 Not Found |
| Update a user | PATCH | `/users/1` | 200 OK |

## Project Structure

```text
postman-user-management-api-testing/
│
├── README.md
├── collections/
│   └── user-management-api.postman_collection.json
└── screenshots/
    └── test-results.png
```

## How to Run the Tests

1. Download and install [Postman](https://www.postman.com/downloads/).
2. Clone or download this GitHub repository.
3. Open Postman.
4. Click **Import** and select the exported collection JSON file from the `collections` folder.
5. Configure the base URL for your User Management API.
6. Open the collection and execute the requests individually, or run all requests using **Collection Runner**.
7. Verify the actual response status codes and response bodies against the expected results.

## API Test Validation

The following validations can be performed in Postman:

- Verify HTTP status codes.
- Check response body structure and required fields.
- Validate user details returned by GET requests.
- Confirm that the POST request creates a user successfully.
- Verify that requesting a nonexistent user returns the expected error response.
- Confirm that the PATCH request updates the specified user's details.

## Test Results

Add a screenshot of your executed Postman tests to the `screenshots/` folder.

**Screenshot:** `screenshots/test-results.png`

> Note: Test results depend on the API implementation. The expected status codes listed above should be confirmed against the actual API responses.

## Learning Outcomes

- Understanding HTTP methods: GET, POST, and PATCH.
- Learning REST API testing fundamentals.
- Validating HTTP response status codes.
- Testing positive and negative scenarios.
- Organizing and exporting Postman collections.
- Documenting API testing projects using GitHub.
