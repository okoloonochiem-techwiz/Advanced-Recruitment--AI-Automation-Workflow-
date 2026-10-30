# Project Overview

## Purpose
Automate the intake and processing of applicant CVs. The workflow receives applications, stores documents, extracts their contents across supported formats, brings in job-description context, processes the information with an AI recruiter agent, and records structured results.

## Business problem
Recruitment teams often receive CVs in different formats. Opening, converting, reading, and transferring applicant information manually creates repetitive administrative work.

## Capabilities visible in the supplied workflow
- Gmail-based resume/application trigger.
- Upload incoming file to Google Drive.
- File-type routing for PDF, text, and Word documents.
- Download and extraction paths for supported file types.
- Word-to-Google-Docs conversion before extraction.
- Retrieval and extraction of a job/application description PDF.
- AI Recruiter Agent connected to an OpenAI Chat Model.
- Structured Output Parser connected to the agent.
- Downstream information extraction and Google Sheets result step.

## Not yet confirmed
The screenshot does not show the exact candidate fields, scoring rubric, prompt, parser schema, or duplicate handling. Confirm these from the exported workflow before documenting them as implemented.
