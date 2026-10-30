# CV Intake and AI Recruitment Screening

## Purpose
Receive applicant documents through Gmail, store them in Google Drive, extract CV content across supported file types, combine it with job-description context, process it with an AI recruiter agent, and send candidate results to Google Sheets.

## Node sequence visible in the screenshot
1. Gmail Trigger Where Resume Drops.
2. Upload File to Drive.
3. Switch for document type routing.
4. PDF path: Get PDF → Text Extractor from PDF.
5. Text path: Get Text → Text Extractor from Text.
6. Word path: Convert Word to Google Doc → Get Google Doc → Text Extractor from converted document.
7. Edit Fields.
8. Application Lookup Description.
9. Text Extractor from Job Description PDF.
10. Recruiter Agent, connected to an OpenAI Chat Model and Structured Output Parser.
11. Information Extractor.
12. Append Candidate Result Here (Google Sheets).

## Folders
- `workflow-export/` — place the n8n JSON export here.
- `screenshots/` — place workflow overview and key node configuration screenshots here.

## To complete
Add the exact agent prompt, parser schema, candidate output fields, job-description lookup logic, spreadsheet mapping, and error handling after inspecting the workflow export.
