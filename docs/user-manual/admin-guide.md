# System Administrator Guide

## Table of Contents
1. [System Overview](#system-overview)
2. [User Management](#user-management)
3. [Company Configuration](#company-configuration)
4. [Module Management](#module-management)
5. [System Maintenance](#system-maintenance)
6. [Security & Access Control](#security--access-control)
7. [Backup & Recovery](#backup--recovery)

## System Overview

### Architecture
The HRMS system uses:
- Multi-tenant architecture
- Separate databases per tenant
- RESTful API backend
- React-based frontend
- MongoDB database

### System Components
- Global database: Company and user management
- Tenant databases: Company-specific data
- API server: Backend services
- Frontend application: User interface

## User Management

### Creating Users
1. Navigate to "Users" → "Add User"
2. Enter user details
3. Assign role (admin, hr, manager, employee)
4. Set permissions
5. Send activation email

### Managing Roles
1. Go to "Users" → "Roles"
2. View existing roles
3. Create custom roles
4. Assign permissions to roles

### User Access Control
1. Configure access levels
2. Set module permissions
3. Manage data access by role

## Company Configuration

### Company Setup
1. Navigate to "Companies" → "Add Company"
2. Enter company details
3. Configure company settings
4. Set up tenant database
5. Initialize default data

### Company Settings
- Company name and details
- Business hours
- Timezone
- Currency
- Statutory settings

## Module Management

### Enabling Modules
1. Go to "Modules" → "Module Management"
2. View available modules
3. Enable/disable modules per company
4. Configure module settings

### Module Configuration
- Leave Management
- Attendance Management
- Payroll
- Biometric Integration
- SAP Integration

## System Maintenance

### Database Management
1. Monitor database performance
2. Perform regular backups
3. Optimize queries
4. Manage indexes

### System Monitoring
1. Monitor system health
2. Track API performance
3. Review error logs
4. Monitor scheduled jobs

### Cron Jobs
- Leave accrual (monthly/yearly)
- Report generation
- Data synchronization
- Cleanup tasks

## Security & Access Control

### Authentication
- JWT-based authentication
- Password policies
- Session management
- Multi-factor authentication (if enabled)

### Authorization
- Role-based access control
- Permission management
- Data access restrictions

### Audit Logs
1. View system audit logs
2. Track user activities
3. Monitor data changes
4. Generate audit reports

## Backup & Recovery

### Backup Strategy
1. Regular database backups
2. File storage backups
3. Configuration backups
4. Test restore procedures

### Recovery Procedures
1. Database restore
2. File restore
3. System recovery
4. Data migration

## Integration Management

### SAP Integration
Refer to: [SAP Integration Guide](../integration/sap-integration-guide.md)

### Biometric Integration
Refer to: [Biometric Integration Guide](../integration/biometric-integration-guide.md)

## Troubleshooting

### Common Issues
1. Database connection issues
2. API errors
3. Performance problems
4. Integration failures

### Log Files
- Application logs
- Error logs
- Access logs
- Integration logs

## Support

For technical support:
- Contact development team
- Email: admin-support@hrms.com
- Refer to integration documentation

---

**Last Updated:** January 2025  
**Version:** 1.0


