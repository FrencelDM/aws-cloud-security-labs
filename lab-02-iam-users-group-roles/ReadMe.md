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
  Policy: AdministratorAccess
- Developers
  Policy: AmazonEC2ReadOnlyAccess

### Roles
- CloudSecurityRole
  - Trusted entity: EC2
  - Permissions: Minimal required access

- ## Security rationale 
Permissions are assigned via groups to simplify access management and auditing. IAM roles are better for services than user. They are used for AWS services to avoid longterm credentials and reduce attack surface. IAM users must create access keys that can leaked or forgotten, and that poses a huge risk until manually remidied.  


## Evidence
- Diagram
<img width="632" height="488" alt="image" src="https://github.com/user-attachments/assets/e4429cf8-d6bf-47f5-b74e-6e670e4cefde" />

- Console screenshots
<img width="1252" height="488" alt="image" src="https://github.com/user-attachments/assets/b6890099-4c39-4042-a798-228c2b22faa5" />

<img width="1252" height="488" alt="image" src="https://github.com/user-attachments/assets/bbffc4f9-97a2-4c20-b658-7199a2705b7b" />

<img width="1206" height="451" alt="image" src="https://github.com/user-attachments/assets/b00063dd-4c61-46e3-bfba-21fdc21485cb" />

<img width="1097" height="464" alt="image" src="https://github.com/user-attachments/assets/ce6269fb-b0f2-4268-9ec7-1dce525ba7a4" />
