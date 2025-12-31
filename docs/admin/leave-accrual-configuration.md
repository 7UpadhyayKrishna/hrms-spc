# Leave Accrual Configuration Guide

## Overview
This guide explains how to configure leave accrual policies in the HRMS system.

## Prerequisites
- Admin or HR role access
- Understanding of company leave policies

## Creating Accrual Policies

### Step 1: Access Accrual Policies
1. Navigate to "Leave Management" → "Accrual Policies"
2. Click "Create Policy"

### Step 2: Configure Basic Settings
- **Leave Type**: Select leave type (Personal Leave, Sick Leave, etc.)
- **Accrual Frequency**: Choose monthly or yearly
- **Accrual Amount**: Enter days to accrue per period
- **Applicable From**: Set effective date

### Step 3: Pro-Rata Configuration
- **Enable Pro-Rata**: Toggle if mid-year joiners should get pro-rata leaves
- **Calculation Method**: 
  - Calendar days
  - Working days
  - Months

### Step 4: Carry Forward Settings
- **Enable Carry Forward**: Allow leaves to carry forward to next year
- **Max Carry Forward**: Maximum days that can be carried forward
- **Expiry Days**: Days after year-end when carried leaves expire

### Step 5: Applicability
- **Applicable To**: 
  - All employees
  - Specific departments
  - Specific designations
  - Specific locations

### Step 6: Save Policy
Click "Save" to create the policy

## Example Configurations

### Monthly Accrual (Personal Leave)
- Frequency: Monthly
- Amount: 1.5 days
- Pro-Rata: Enabled
- Carry Forward: Enabled (max 10 days)

### Yearly Accrual (Sick Leave)
- Frequency: Yearly
- Amount: 12 days
- Pro-Rata: Enabled
- Carry Forward: Disabled

## Manual Accrual Processing

### Monthly Accrual
1. Go to "Leave Management" → "Accrual" → "Monthly"
2. Select month and year
3. Click "Process Accrual"
4. Review results

### Yearly Accrual
1. Go to "Leave Management" → "Accrual" → "Yearly"
2. Select year
3. Click "Process Accrual"
4. Review results

## Year-End Processing

### Carry Forward Processing
1. Navigate to "Leave Management" → "Accrual" → "Year-End"
2. Select previous year
3. Process carry forward based on policies
4. Review and approve carry forward amounts

### Lapse Processing
1. Leaves exceeding max carry forward are lapsed
2. Review lapsed leaves report
3. Update leave balances

## Historical Data Migration

### Upload Historical Data
1. Prepare Excel file with format:
   - Employee Email
   - Leave Type
   - Year
   - Total, Consumed, Available
2. Go to "Leave Management" → "Accrual" → "Historical Upload"
3. Upload Excel file
4. Review and confirm import

## Best Practices

1. **Configure at Year Start**: Set up all accrual policies before the year begins
2. **Test Policies**: Test accrual calculations before applying to all employees
3. **Document Policies**: Maintain documentation of accrual rules
4. **Regular Monitoring**: Review accrual results monthly
5. **Year-End Planning**: Plan year-end processing in advance

## Troubleshooting

### Accrual Not Processing
- Check if policy is active
- Verify applicable date
- Check employee eligibility

### Incorrect Calculations
- Review pro-rata settings
- Verify joining dates
- Check policy applicability

## Support

For assistance:
- Contact HR team
- Email: hr-support@hrms.com

---

**Last Updated:** January 2025


