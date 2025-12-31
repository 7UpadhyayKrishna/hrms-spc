# Approval Workflow Setup Guide

## Overview
This guide explains how to configure multi-level approval workflows for leave requests, encashment, and other entities.

## Prerequisites
- Admin or HR role access
- Understanding of approval hierarchy

## Creating Approval Workflows

### Step 1: Access Workflows
1. Navigate to "Approval Workflow" → "Workflows"
2. Click "Create Workflow"

### Step 2: Basic Configuration
- **Entity Type**: Select (LeaveRequest, LeaveEncashment, ProfileUpdateRequest)
- **Workflow Name**: Enter descriptive name
- **Description**: Add workflow description

### Step 3: Define Approval Levels
For each level:
- **Level Number**: Sequential level (1, 2, 3...)
- **Approver Type**: 
  - Manager (reporting manager)
  - HR
  - Role (specific role)
  - User (specific user)
- **Min Approvals**: Minimum approvals required at this level
- **Required**: Is this level mandatory?

### Step 4: SLA Configuration
- **SLA Minutes**: Time limit for approval at each level
- **Default**: 1440 minutes (24 hours)

### Step 5: Escalation Rules
- **Enable Escalation**: Toggle escalation
- **Escalate To**: Who to escalate to
- **Escalate After Minutes**: Time before escalation
- **Max Escalations**: Maximum escalation count

### Step 6: Save Workflow
Click "Save" to create workflow

## Approval Matrix Configuration

### Step 1: Create Approval Matrix
1. Go to "Approval Workflow" → "Approval Matrix"
2. Click "Create Matrix"

### Step 2: Define Criteria
- **Entity Type**: Select entity type
- **Criteria**: JSON object with conditions
  - Example: `{ "leaveType": "Personal Leave", "numberOfDays": { "$gte": 5 } }`
- **Workflow**: Select applicable workflow
- **Priority**: Lower number = higher priority

### Step 3: Save Matrix
Click "Save"

## Example Workflows

### Simple Leave Approval (2 Levels)
- Level 1: Manager (required)
- Level 2: HR (required)
- SLA: 24 hours per level

### Complex Leave Approval (3 Levels)
- Level 1: Manager (required)
- Level 2: Department Head (required)
- Level 3: HR (required)
- SLA: 24 hours per level
- Escalation: After 48 hours to HR Head

## Delegation Setup

### Creating Delegation
1. Navigate to "Approval Workflow" → "Delegations"
2. Click "Create Delegation"
3. Select delegate
4. Set start and end dates
5. Choose entity types
6. Add reason
7. Save

### Managing Delegations
- View active delegations
- Edit or cancel as needed
- Track delegation history

## Testing Workflows

### Test Scenarios
1. Create test leave request
2. Verify approval routing
3. Test escalation
4. Verify SLA tracking
5. Test delegation

## Best Practices

1. **Define Clear Hierarchy**: Establish clear approval chain
2. **Set Realistic SLAs**: Set achievable SLA targets
3. **Enable Escalation**: Configure escalation for critical requests
4. **Document Workflows**: Maintain workflow documentation
5. **Regular Review**: Review and optimize workflows periodically

## Troubleshooting

### Requests Not Routing Correctly
- Check approval matrix criteria
- Verify workflow assignment
- Review employee hierarchy

### Escalation Not Working
- Verify escalation rules
- Check escalation recipient
- Review SLA settings

## Support

For assistance:
- Contact HR team
- Email: hr-support@hrms.com

---

**Last Updated:** January 2025


