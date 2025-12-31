# Biometric Integration Setup Guide

## Overview
This guide explains how to integrate biometric devices with the HRMS system.

## Prerequisites
- Admin or HR role access
- Biometric device access
- Network connectivity

## Device Registration

### Step 1: Add Device
1. Navigate to "Attendance" → "Biometric Devices"
2. Click "Add Device"

### Step 2: Device Configuration
- **Device Name**: Enter descriptive name
- **Device Type**: Select (ZKTeco, eSSL, etc.)
- **IP Address**: Device IP address
- **Port**: Communication port
- **Location**: Device location
- **Serial Number**: Device serial number

### Step 3: Connection Test
1. Click "Test Connection"
2. Verify connection status
3. Save device

## Employee Sync

### Syncing Employees to Device
1. Go to "Biometric Devices" → Select device
2. Click "Sync Employees"
3. Select employees to sync
4. Click "Sync"
5. Verify sync status

### Employee Onboarding
- New employees are automatically synced (if enabled)
- Manual sync available for existing employees

## Attendance Data Pull

### Manual Data Pull
1. Navigate to "Biometric Devices" → Select device
2. Click "Pull Attendance"
3. Select date range
4. Click "Pull Data"
5. Review pulled records

### Automatic Data Sync
- Configure automatic sync schedule
- Set sync frequency (hourly, daily)
- Monitor sync logs

## Data Validation

### Validating Attendance Records
1. Go to "Attendance" → "Biometric Data"
2. Review pulled records
3. Validate check-in/check-out times
4. Process valid records
5. Handle exceptions

## Device Management

### Updating Device Settings
1. Select device
2. Click "Edit"
3. Update settings
4. Save changes

### Removing Device
1. Select device
2. Click "Remove"
3. Confirm removal

## Troubleshooting

### Connection Issues
- Verify IP address and port
- Check network connectivity
- Review firewall settings
- Test device accessibility

### Sync Failures
- Check device status
- Verify employee data
- Review sync logs
- Retry sync operation

### Data Validation Errors
- Review data format
- Check time zones
- Verify employee mapping
- Handle exceptions manually

## Best Practices

1. **Regular Sync**: Schedule regular data pulls
2. **Monitor Logs**: Review sync logs regularly
3. **Validate Data**: Validate attendance data before processing
4. **Handle Exceptions**: Process exceptions promptly
5. **Maintain Devices**: Keep devices updated and maintained

## Support

For assistance:
- Contact device vendor
- Email: hr-support@hrms.com
- Refer to device-specific documentation

---

**Last Updated:** January 2025


