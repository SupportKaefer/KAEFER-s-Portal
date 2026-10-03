# Security Policy

## Reporting a Security Issue

Please do not report vulnerabilities or disclose employee information in public GitHub issues, discussions or pull requests.

Contact the portal maintainer privately through an established support channel. Include the affected feature, steps to reproduce the issue and its potential impact. Use fictional or redacted examples.

Never include passwords, PINs, private tracking links, setup codes or employee records.

## Access Control

- Employee ticket details and conversations require successful backend verification.
- Staff accounts require superadmin approval.
- Staff access is restricted according to role, approved projects and ticket assignments.
- Backend permission checks must apply to every protected operation.
- A supplied email address alone is not proof of identity.
- Staff must use individual accounts and keep credentials private.

## Data Protection

- Collect only information needed for the requested service.
- Keep employee records, authentication secrets and confidential configuration out of public repositories.
- Do not store new passwords or PINs as readable text.
- Do not publish generated employee forms or sensitive attachments through public links.
- Restrict direct access to the underlying Google Sheet.
- Avoid recording credentials or private tracking tokens in logs.

## Record Preservation

Updates must not delete or overwrite previously recorded employee data as part of setup or migration.

Changes should preserve ticket conversations, assignments and activity history. Any correction to a business record should be authorized and recorded.

Activity records are append-only through the portal, but are not tamper-proof against people with direct Sheet edit access.

## Security Review

Changes affecting authentication, permissions, ticket tracking, form generation or data storage must be reviewed before deployment.

Review should include unauthorized access attempts, malformed requests, expired sessions, duplicate submissions and accidental exposure of sensitive information.

## Incident Response

If a security incident is suspected, the maintainer should restrict affected access, preserve relevant evidence, investigate the scope and rotate exposed credentials or tokens where appropriate.

Affected users should receive clear guidance when action is required.
