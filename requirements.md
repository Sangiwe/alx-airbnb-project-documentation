# Backend Feature Requirements Specification

## 1. User Authentication System

### Functional Requirements
- Allow users to register with email/password or OAuth providers (Google/Facebook)
- Enable JWT-based authentication for subsequent requests
- Implement role-based access control (guest, host, admin)
- Support password reset functionality

### Technical Specifications

#### API Endpoints
| Method | Endpoint          | Description                     |
|--------|-------------------|---------------------------------|
| POST   | `/api/auth/register` | Register new user              |
| POST   | `/api/auth/login`    | Login with credentials         |
| POST   | `/api/auth/oauth`    | OAuth authentication           |
| POST   | `/api/auth/refresh`  | Refresh JWT token              |
| POST   | `/api/auth/logout`   | Invalidate JWT token           |

#### Input/Output
**Registration (POST /api/auth/register)**
```json
// Request
{
  "email": "user@example.com",
  "password": "SecurePass123!",
  "first_name": "John",
  "last_name": "Doe",
  "role": "guest"
}

// Response (201 Created)
{
  "id": "a1b2c3d4-e5f6-7890-g1h2-i3j4k5l6m7n8",
  "email": "user@example.com",
  "role": "guest",
  "access_token": "eyJhbGciOi...",
  "refresh_token": "eyJhbGciOi..."
}