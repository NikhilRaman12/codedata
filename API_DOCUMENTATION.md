# API Documentation

## Overview
This document describes the API endpoints available in the codedata repository. Each endpoint provides functionality to interact with the application's core features.

## Endpoints

### 1. Get User Information
- **Endpoint:** `/api/user`
- **Method:** `GET`
- **Description:** Retrieves the information of the currently authenticated user.
- **Request Example:**  
```bash
curl -X GET https://api.example.com/api/user -H 'Authorization: Bearer {token}'
```
- **Response Example:**  
```json
{
  "id": 123,
  "name": "John Doe",
  "email": "john.doe@example.com"
}
```

### 2. Update User Information
- **Endpoint:** `/api/user`
- **Method:** `PUT`
- **Description:** Updates the information of the currently authenticated user.
- **Request Example:**  
```bash
curl -X PUT https://api.example.com/api/user -H 'Authorization: Bearer {token}' -H 'Content-Type: application/json' -d '{"name": "Jane Doe"}'
```
- **Response Example:**  
```json
{
  "success": true,
  "message": "User information updated successfully."
}
```

### 3. Get All Users
- **Endpoint:** `/api/users`
- **Method:** `GET`
- **Description:** Retrieves a list of all users in the system.
- **Request Example:**  
```bash
curl -X GET https://api.example.com/api/users -H 'Authorization: Bearer {token}'
```
- **Response Example:**  
```json
[
  {
    "id": 123,
    "name": "John Doe",
    "email": "john.doe@example.com"
  },
  {
    "id": 124,
    "name": "Jane Doe",
    "email": "jane.doe@example.com"
  }
]
```

## Conclusion
This document provides a brief overview of the available API endpoints. For more details on responses and potential error messages, please refer to the source code or further documentation.