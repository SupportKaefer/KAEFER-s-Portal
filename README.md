# KAEFER Employee Help Portal

An independently maintained, multilingual portal that helps employees access notices, estimate overtime earnings, prepare forms and communicate with support.

**Live portal:** https://supportkaefer.github.io/KAEFER-s-Portal/

**Maintained by:** Jitendra Bhujel  
**Updated:** 3 October 2026

## Employee Services

### Digital Noticeboard
A homepage for employee announcements and updates, with notice content managed through Google Sheets.

### Overtime & Payslip Calculator
Estimate salary and overtime earnings using the existing 240-hour monthly basis and 25th-day cutoff.

Supports normal, holiday and retro overtime at 1.5× the base rate, bonus overtime at 1.0×, and allowances. Results are estimates before deductions, not official payroll figures.

### Next of Kin & Nomination Form
Enter declarant and nominee details and download the form for printing. Required signatures, witness details and dates must be completed manually.

### Support Requests
Submit salary or site concerns and receive a ticket number for follow-up.

### Private Ticket Tracking
Access requests using the ticket number, registered mobile number and personal PIN. Existing private tracking links remain supported.

Ticket details and conversations are shown only after successful backend verification.

### Conversation Timeline
Follow employee and support messages with timestamps and sender labels in the dedicated Track Request tab.

## Support Team Dashboard

Approved staff can:

- Review tickets permitted by their project access or ticket assignment.
- Reply to employees and update request status.
- Assign or forward tickets to responsible staff.
- View ticket activity and team workload summaries.
- Request access to multiple projects.

Superadmin can manage staff approvals, roles, project permissions, employee project mappings and password assistance.

Staff use a separate portal username and password. Registration requires approval; a supplied Gmail address alone does not grant access.

## Accessibility

- English, Nepali, Hindi, Arabic and Urdu.
- Right-to-left layouts for Arabic and Urdu.
- Responsive layouts for phones, tablets and desktops.
- Separate Home, OT Calculator, Forms, New Request and Track Request tabs.
- Progress messages and disabled buttons while requests are processing.

## Benefits

- Gives employees one place to find information and request help.
- Makes ticket progress and previous conversations easier to follow.
- Helps support staff coordinate ownership and responses.
- Reduces routine direct editing of the Google Sheet.
- Records actions, assignments and status changes for accountability.

## Data Handling

Updates are designed to preserve previously recorded Sheet data.

Ticket access and staff permissions are checked by the backend. Duplicate protection helps prevent repeated submissions, and activity records document who performed an action and when.

Activity records are append-only through the portal. People with direct edit access to the underlying Sheet can still alter its contents, so spreadsheet access must remain restricted.

## Technology

- **Frontend:** HTML, CSS and JavaScript hosted on GitHub Pages.
- **Backend:** Google Apps Script.
- **Data storage:** Google Sheets.

Performance and availability depend on network conditions and Google Apps Script quotas.

## Important Notice

This portal is independently maintained and is not an official KAEFER company system.

Calculator results are for reference only. Official salary and payroll figures remain subject to company processing.

Never share passwords, PINs, confidential setup codes or private tracking links in public repository files or issues.
