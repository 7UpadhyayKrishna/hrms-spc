# Data Migration Guide

## Overview
This guide explains how to migrate historical data into the HRMS system.

## Prerequisites
- Admin access
- Data in Excel/CSV format
- Data validation completed

## Employee Data Migration

### Format
- Employee Code
- First Name, Last Name
- Email
- Department
- Designation
- Joining Date
- Other fields

### Process
1. Prepare Excel file
2. Validate data
3. Upload via migration script
4. Review results
5. Confirm import

## Leave Data Migration

### Format
- Employee Email
- Leave Type
- Year
- Total, Consumed, Available

### Process
1. Prepare Excel file
2. Run migration script
3. Review accrual calculations
4. Confirm import

## Attendance Data Migration

### Format
- Employee Code
- Date
- Check-in, Check-out
- Status

### Process
1. Prepare Excel file
2. Validate dates
3. Run migration script
4. Review results

## Migration Scripts

### Employee Migration
Location: `hrms-backend/src/scripts/migrateEmployees.js`

### Leave Migration
Location: `hrms-backend/src/scripts/migrateLeaveHistory.js`

### Attendance Migration
Location: `hrms-backend/src/scripts/migrateAttendance.js`

## Best Practices

1. **Backup First**: Backup existing data
2. **Validate Data**: Validate before migration
3. **Test Migration**: Test with sample data
4. **Review Results**: Review migration results
5. **Document Changes**: Document any data transformations

---

**Last Updated:** January 2025


