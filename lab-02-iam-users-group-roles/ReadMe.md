# lab 02 - Iam users, group, and roles

## Obecjtive 
Implementing identity seperation, governance, and least-privilege access using IAM

## Actions performed 
- Created admistrative and stantard IAM users
- Assigned permissons using IAM groups
- Implemented Amazon EC2 read-only access for developpers
- Created an IAM role for AWS Services

## IAM Configuration

### Users
- admin-user
- developer-user

### Groups
- Admins
  - Policy: AdministratorAccess
- Developers
  - Policy: AmazonEC2ReadOnlyAccess

### Roles
- CloudSecurityRole
  - Trusted entity: EC2
  - Permissions: Minimal required access

- ## Security rationale
Permissions are assigned via groups to simplify access management and auditing. IAM roles are used for AWS services to avoid longterm credentials and reduce attack surface.

## Evidence
- Diagram


- Console screenshots
