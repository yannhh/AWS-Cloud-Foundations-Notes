# Module 4: Securing Accounts

Favorite: No
Archive: No
Notebook: AWS Cloud  (../../AWS%20Cloud%2035b6c6880dca809b964ce3b71f757313.md)
Edited: May 10, 2026 6:40 PM
Created: May 10, 2026 6:19 PM

## AWS Organizations

- Allows you to consolidate multiple AWS accounts so that you can centrally manage them.
- Security features of AWS Organizations:
    - Group AWS accounts into Organizational units (OUs) and attach different access policies to each OU.
    - Integrations and Support for IAM
        - Permissions to a user are the intersection of what is allows by AWS Organizations and what is granted by IAM in that account.
    - Use service control policies to establish control over the AWS services and API actions that each AWS account can access.

## AWS Organizations: Service Control Policies

- Service Control Policies (SCPs) offer centralized control over accounts.
    - Limit permissions that are available in an account that is part of an organization.
- Ensures that accounts comply with access control guidelines.
- SCPS are similar to IAM permissions policies -
    - They use similar syntax.
    - However, an SCP never grants permissions.
    - Instead, SCPs specify the maximum permissions for an organization.

## AWS Key Management Service (AWS KMS)

Features:

- Allows creation and management of encryption keys.
- Allows control the use of encryption across AWS services and in applications.
- Integrates with AWS CloudTrail to log all key usage.
- Uses hardware security modules (HSMs) that are validated by Federal Information Processing Standards (FIPS) 140-2 to protect keys.

## Amazon Cognito

Features:

- Adds user sign-up, sign-in, and access control to web and mobile applications.
- Scales to millions of users.
- Supports sign-in with social identity providers, like Facebook, Google, and Amazon; and enterprise identity providers, such as Microsoft Active Directory via Security Assertion Markup Language (SAML) 2.0.

## AWS Shield

Features:

- Managed distributed denial of service (DDOS) protection service.
- Safeguards applications running on AWS.
- Provides always-on detection and automatic inline mitigations.
- AWS Shield Standard enabled for at no additional cost. AWS Shield Advanced is an optional paid service.
- It is used to minimize application downtime and latency