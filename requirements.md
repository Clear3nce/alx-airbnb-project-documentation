# Airbnb Clone - Backend Specification

## Table of Contents
1. [User Authentication](#1-user-authentication)
2. [Property Management](#2-property-management) 
3. [Booking System](#3-booking-system)
4. [Technical Architecture](#4-technical-architecture)
5. [API Summary](#5-api-summary)

---

## 1. User Authentication

### 1.1 Functional Requirements
- ✅ User registration (guest/host roles)
- ✅ Email/password login
- 🔐 JWT authentication
- ⚙️ OAuth 2.0 (Google/Facebook)
- ✉️ Email verification flow
- 🔄 Password reset functionality

### 1.2 API Endpoints

#### `POST /api/v1/auth/register`
**Request:**
```json
{
  "first_name": "John",
  "last_name": "Doe",
  "email": "john@example.com",
  "password": "SecurePass123!",
  "role": "guest",
  "phone": "+254712345678"
}
