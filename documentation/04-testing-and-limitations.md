# Testing and Limitations

## Suggested test plan

| Test | Verify |
|---|---|
| PDF CV | PDF route selected and text extracted |
| Text CV | Text route selected and content extracted |
| Word CV | Conversion succeeds and converted document text is extracted |
| Unsupported/missing attachment | Error or fallback behaviour is understood |
| Job description | Correct source document is retrieved and extracted |
| AI processing | Agent receives the intended candidate and job context |
| Structured output | Agent response conforms to parser schema |
| Google Sheets | Candidate result is written to intended columns |
| Repeated application | Duplicate handling is tested; it is not assumed |

## Documentation limitations
The screenshot shows the node layout, but not complete node settings, prompt text, parser schema, spreadsheet columns, or execution logs. These details require the exported workflow and test runs.

## Responsible use
- Keep a human recruiter responsible for decisions.
- Review AI outputs for errors and unsupported conclusions.
- Avoid using protected or sensitive characteristics as screening criteria.
- Restrict access to applicant documents and follow an appropriate retention policy.
- Test for inconsistent outcomes across CV formats and writing styles.
