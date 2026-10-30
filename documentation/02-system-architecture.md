# System Architecture

## High-level flow
Gmail receives the application. The file is uploaded to Google Drive and routed according to its type.

### Document paths
- **PDF:** Get PDF from Drive → extract text from PDF.
- **Text:** Get text from Drive → extract text from text file.
- **Word:** Convert Word to Google Docs → retrieve converted document → extract text.

The extracted candidate content is prepared and combined with job-description context retrieved from Google Drive. The AI Recruiter Agent uses an OpenAI Chat Model and a Structured Output Parser. A downstream information extraction step prepares the result for Google Sheets.

## Integrations

| Component | Visible role |
|---|---|
| Gmail | Application/resume trigger |
| Google Drive | Stores applicant files and provides job-description source |
| Google Docs | Word document conversion path |
| Extraction nodes | Extract content from candidate and job-description documents |
| OpenAI Chat Model | Language model connected to the recruiter agent |
| Recruiter Agent | Processes candidate and job context |
| Structured Output Parser | Structures agent response |
| Google Sheets | Candidate result destination |

See [system organogram](../diagrams/system-organogram.md).

## Configuration details to confirm
Gmail filters, Drive folder IDs, MIME-type switch rules, job-description lookup criteria, agent prompt, output schema, Sheets column mapping, error handling, and duplicate application behaviour.
