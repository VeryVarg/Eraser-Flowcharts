# Example Flowchart: Simple Login Flow

This is an example flowchart demonstrating how to document your Eraser.io diagrams.

```
// Eraser.io Diagram Code
// This represents a simple user login flow

Start [shape: oval]
Enter Credentials [shape: rectangle]
Validate Credentials [shape: diamond, label: "Valid?"]
Check 2FA [shape: diamond, label: "2FA Enabled?"]
Send 2FA Code [shape: rectangle]
Enter 2FA Code [shape: rectangle]
Verify 2FA [shape: diamond, label: "Code Valid?"]
Grant Access [shape: rectangle]
Deny Access [shape: rectangle]
End [shape: oval]

Start > Enter Credentials
Enter Credentials > Validate Credentials
Validate Credentials > Check 2FA [label: "Yes"]
Validate Credentials > Deny Access [label: "No"]
Check 2FA > Send 2FA Code [label: "Yes"]
Check 2FA > Grant Access [label: "No"]
Send 2FA Code > Enter 2FA Code
Enter 2FA Code > Verify 2FA
Verify 2FA > Grant Access [label: "Yes"]
Verify 2FA > Deny Access [label: "No"]
Grant Access > End
Deny Access > End
```

## Overview

This flowchart represents a user authentication flow with optional two-factor authentication (2FA).

## Details

- **Created**: 2025-11-23
- **Last Updated**: 2025-11-23
- **Author**: Repository Maintainer
- **Category**: Authentication & Security
- **Type**: Process Flow

## Description

This flowchart illustrates the complete login process for a system with optional 2FA:

1. **User Entry**: User enters their credentials (username/password)
2. **Validation**: System validates the credentials against stored data
3. **2FA Check**: If 2FA is enabled for the account, proceed to 2FA verification
4. **2FA Process**: 
   - Send verification code to user's registered device
   - User enters the received code
   - System verifies the code
5. **Access Decision**: Grant or deny access based on validation results

### Key Decision Points

- **Credential Validation**: Checks if username and password match stored records
- **2FA Status**: Determines if additional authentication is required
- **2FA Code Verification**: Validates the one-time code provided by the user

## Files

- **Diagram Source**: `flowcharts/examples/simple-login-flow.md`
- **Exported Image**: (Export from Eraser.io and add to `exports/examples/`)

## Use Cases

This pattern is commonly used in:
- Web applications
- Mobile apps
- API authentication systems
- Enterprise software

## Notes

This is a simplified example. Production systems should include:
- Rate limiting for failed attempts
- Account lockout mechanisms
- Password reset flows
- Session management
- Audit logging

## Related Flowcharts

- Password Reset Flow (example)
- User Registration Flow (example)
- Session Management (example)
