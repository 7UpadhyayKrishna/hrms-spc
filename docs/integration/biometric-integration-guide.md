# Biometric Integration Guide

## Overview
This guide details the biometric device integration architecture and implementation.

## Supported Devices

### ZKTeco
- Device models: Various ZKTeco models
- Communication: TCP/IP
- Protocol: ZKTeco SDK

### eSSL
- Device models: Various eSSL models
- Communication: TCP/IP
- Protocol: eSSL SDK

## Integration Architecture

```
HRMS System          Biometric Device
    │                    │
    │───TCP/IP──────────>│
    │<───Attendance──────│
    │                    │
```

## Device Registration

### Configuration
- Device Name
- IP Address
- Port
- Device Type
- Location

### Connection
- Test connection
- Verify device status
- Register device

## Employee Sync

### Sync Process
1. Connect to device
2. Send employee data
3. Register fingerprints
4. Verify sync status

### Data Format
- Employee ID
- Name
- Department
- Fingerprint data

## Attendance Data Pull

### Pull Process
1. Connect to device
2. Request attendance data
3. Receive records
4. Validate data
5. Store in HRMS

### Data Validation
- Check employee mapping
- Validate timestamps
- Handle duplicates
- Process exceptions

## Implementation Details

### Base Adapter
Location: `hrms-backend/src/services/biometric/BaseAdapter.js`

### ZKTeco Adapter
Location: `hrms-backend/src/services/biometric/ZKTecoAdapter.js`

### eSSL Adapter
Location: `hrms-backend/src/services/biometric/eSSLAdapter.js`

## Error Handling

### Connection Errors
- Retry mechanism
- Error logging
- Notification alerts

### Data Validation
- Timestamp validation
- Employee mapping checks
- Duplicate detection

## Best Practices

1. **Regular Sync**: Schedule regular data pulls
2. **Monitor Logs**: Review sync logs regularly
3. **Validate Data**: Validate attendance data before processing
4. **Handle Exceptions**: Process exceptions promptly
5. **Maintain Devices**: Keep devices updated and maintained

---

**Last Updated:** January 2025


