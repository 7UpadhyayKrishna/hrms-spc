# API Documentation

## Base URL
```
Production: https://api.hrms.com
Development: http://localhost:5000
```

## Authentication

### Login
```http
POST /api/auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "password"
}
```

### Response
```json
{
  "success": true,
  "token": "jwt_token_here",
  "user": { ... }
}
```

## Leave Management APIs

### Get Leave Balance
```http
GET /api/leave/balance
Authorization: Bearer {token}
```

### Apply Leave
```http
POST /api/leave/apply
Authorization: Bearer {token}
Content-Type: application/json

{
  "leaveType": "Personal Leave",
  "startDate": "2025-02-01",
  "endDate": "2025-02-03",
  "reason": "Personal work"
}
```

## Leave Encashment APIs

### Check Eligibility
```http
POST /api/leave-encashment/check-eligibility
Authorization: Bearer {token}
Content-Type: application/json

{
  "leaveType": "Personal Leave",
  "numberOfDays": 5
}
```

### Create Encashment Request
```http
POST /api/leave-encashment/requests
Authorization: Bearer {token}
Content-Type: application/json

{
  "leaveType": "Personal Leave",
  "numberOfDays": 5,
  "reason": "Financial need"
}
```

## Reports APIs

### Leave Entitlement Report
```http
GET /api/reports/leave/entitlement?year=2025&export=excel
Authorization: Bearer {token}
```

### Attendance Summary Report
```http
GET /api/reports/attendance/summary?startDate=2025-01-01&endDate=2025-01-31
Authorization: Bearer {token}
```

## Analytics APIs

### Attendance Trends
```http
GET /api/reports/analytics/attendance?startDate=2025-01-01&endDate=2025-01-31&groupBy=month
Authorization: Bearer {token}
```

### Leave Patterns
```http
GET /api/reports/analytics/leave?startDate=2025-01-01&endDate=2025-01-31
Authorization: Bearer {token}
```

## Error Responses

### 400 Bad Request
```json
{
  "success": false,
  "message": "Validation error"
}
```

### 401 Unauthorized
```json
{
  "success": false,
  "message": "Unauthorized"
}
```

### 500 Internal Server Error
```json
{
  "success": false,
  "message": "Internal server error"
}
```

## Rate Limiting
- 100 requests per minute per user
- 1000 requests per hour per user

## Pagination
```http
GET /api/resource?page=1&limit=20
```

## Filtering
```http
GET /api/resource?field=value&sort=field:asc
```

---

**Last Updated:** January 2025


