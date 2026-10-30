# Setup and Configuration

This is a setup checklist based on the visible workflow. Exact node parameters must be confirmed from the n8n JSON export.

## Prerequisites
- n8n instance
- Gmail OAuth credential
- Google Drive and Google Sheets credentials
- Google Docs permissions for Word conversion
- OpenAI API credential

## Setup sequence
1. Import the workflow JSON export into n8n.
2. Configure the Gmail trigger and confirm how attachments are handled.
3. Connect Google Drive and select the applicant upload and job-description locations.
4. Verify the file-type switch rules for PDF, text, and Word files.
5. Verify Word-to-Google-Docs conversion and document extraction permissions.
6. Connect the OpenAI Chat Model and review the Recruiter Agent prompt.
7. Confirm the Structured Output Parser schema.
8. Map the candidate result fields to the correct Google Sheets columns.
9. Test with sample CVs in each supported format before enabling real applications.

## Security
Store credentials in n8n's credential manager. Never commit API keys, OAuth tokens, private webhook URLs, real CVs, or applicant personal information.
