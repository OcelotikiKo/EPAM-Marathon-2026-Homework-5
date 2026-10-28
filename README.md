# EPAM IT Marathon 2026 вЂ“ Backend Homework #5

Backend homework completed as part of **EPAM IT Marathon 2026**.

## Live Demo

**[Green Tasty Restaurant вЂ“ Open Website](https://dl8v07zbkza4a.cloudfront.net/main)**

The application is deployed using AWS Lambda, Amazon API Gateway, Amazon DynamoDB and Amazon CloudFront.

## Implemented Functionality

### Level 1 вЂ“ Group Pre-Order Overview

`GET /guest/groups/{groupReservationId}/sessions`

Allows the reservation owner to view participants, selected dishes, quantities, individual totals and submission statuses.

### Level 2 вЂ“ Owner Session and Order Consolidation

`GET /reservations/{reservationId}/guest-session-id`

`POST /group-reservations/{groupReservationId}/submit`

Retrieves the owner's guest session ID and consolidates submitted guest orders into the restaurant order.

### Level 3 вЂ“ Guest Session Management

`DELETE /guest/groups/{groupReservationId}/sessions/{guestSessionId}`

Allows the reservation owner to remove a guest session and receive an updated group snapshot. Owner sessions are protected from deletion.

## Testing

- **157 unit tests passed**
- AWS Lambda deployment verified
- API endpoints tested using AWS and DynamoDB
- Group pre-order submission and guest removal verified

## Technologies

- C# / .NET 10
- AWS Lambda
- Amazon API Gateway
- Amazon DynamoDB
- Amazon Cognito
- xUnit
- Git / GitHub

## Repository Contents

This submission contains the backend source code and automated tests relevant to the homework. Deployment infrastructure, environment-specific configuration and credentials are excluded.
