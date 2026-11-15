# Restful Booker API Testing

## Project Overview
This project documents API testing conducted using Postman on the Restful Booker API as part of a QA Technical Assessment.

## Tools Used
- Postman
- Restful Booker API

## API Endpoints Tested

| Method | Endpoint | Description |
|---|---|---|
| POST | `/auth` | Generate authentication token |
| POST | `/booking` | Create a booking |
| GET | `/booking/{id}` | Retrieve booking details |
| GET | `/booking` | Retrieve booking IDs |
| PUT | `/booking/{id}` | Update booking details |
| PATCH | `/booking/{id}` | Partially update booking details |
| DELETE | `/booking/{id}` | Delete a booking |

## Test Scenarios
- Authentication and token generation
- Booking creation and booking ID extraction
- Retrieval and verification of booking information
- Full and partial booking updates
- Booking deletion
- Negative testing for incomplete booking requests
- Invalid data type testing
- Unauthorized PUT request without authentication

## Test Automation and Validation
Postman scripts were used to verify response status codes, extract and save authentication tokens and booking IDs, and validate the JSON schema of the booking creation response.

## Negative Testing Results
- Unauthorized PUT request: HTTP 403 Forbidden; both assertions passed.
- Invalid booking data: HTTP 500 Internal Server Error; one of the two assertions failed because the response did not return the expected client-error status.
- Incomplete booking request: HTTP 500 Internal Server Error was observed.

## Repository Contents
- Postman request files
- Part 3 API Testing Documentation Report

## How to Import and Run
1. Download the Postman request files from this repository.
2. Open Postman and select Import.
3. Import the available request files.
4. Review authentication settings and required variables.
5. Execute the requests individually.

