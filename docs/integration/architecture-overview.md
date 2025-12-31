# System Architecture Overview

## Architecture Diagram

```
┌─────────────────┐
│   Frontend      │
│   (React)       │
└────────┬────────┘
         │
         │ HTTP/REST
         │
┌────────▼────────┐
│   API Server    │
│   (Node.js)     │
└────────┬────────┘
         │
    ┌────┴────┐
    │         │
┌───▼───┐ ┌──▼──────┐
│Global │ │ Tenant  │
│  DB   │ │   DBs   │
└───────┘ └─────────┘
```

## System Components

### Frontend
- **Technology**: React.js
- **Location**: `hrms-frontend/`
- **Features**: 
  - User interface
  - Dashboard
  - Forms and reports
  - Responsive design

### Backend API
- **Technology**: Node.js, Express.js
- **Location**: `hrms-backend/`
- **Features**:
  - RESTful APIs
  - Authentication/Authorization
  - Business logic
  - Data validation

### Database
- **Technology**: MongoDB
- **Structure**:
  - Global database: Company and user management
  - Tenant databases: Company-specific data (one per company)

## Multi-Tenant Architecture

### Global Database
Stores:
- Companies
- Global users (super admin)
- Modules
- Packages

### Tenant Databases
Each company has separate database:
- Employee data
- Leave records
- Attendance records
- Work schedules
- Company-specific configurations

## Data Flow

### Authentication Flow
1. User login → API validates credentials
2. JWT token generated
3. Token used for subsequent requests
4. Tenant context determined from user

### Request Flow
1. Frontend sends request with token
2. API validates token
3. Tenant middleware determines company
4. Request routed to tenant database
5. Response sent back to frontend

## Security

### Authentication
- JWT-based authentication
- Token expiration
- Refresh tokens

### Authorization
- Role-based access control
- Permission-based authorization
- Data isolation per tenant

## Integration Points

### SAP Integration
- RFC/BAPI connections
- Employee master data sync
- Leave balance sync
- Attendance data sync

### Biometric Integration
- Device communication protocols
- Employee sync to devices
- Attendance data pull
- Data validation

## Scalability

### Horizontal Scaling
- API servers can be scaled horizontally
- Load balancer distributes requests
- Database sharding for large tenants

### Performance Optimization
- Database indexing
- Query optimization
- Caching strategies
- Connection pooling

## Deployment

### Environment Setup
- Development
- Staging
- Production

### Infrastructure
- Application servers
- Database servers
- File storage
- Email service

---

**Last Updated:** January 2025


