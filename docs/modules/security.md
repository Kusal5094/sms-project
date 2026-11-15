# Security module

Owner: kavinsu-1234
Branch: feature/security-testing

## Covers
- Login authentication
- Pre-approved user registration
- Role-based routing
- Row Level Security (RLS)
- Audit logs

## Tables
- profiles
- allowed_users
- audit_logs

## How to test
1. Register with an email that is not on the allowed list (should be refused).
2. Sign in as admin and as teacher and compare the dashboards.
3. Open an admin page while signed in as a teacher (should be blocked).
4. Check that a teacher cannot read another teacher's data.
