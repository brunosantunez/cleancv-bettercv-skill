# ATS CV Generator

An AI tool designed to create or modify resumes optimized for Applicant Tracking Systems (ATS) and crafted to capture the attention of human recruiters.

## What it does

- **Mode A:** Creates a resume from scratch using raw data and a specific job description.
- **Mode B:** Analyzes your existing resume, identifies formatting or keyword issues, and rewrites it to align with a specific job description.

## Features

- Extracts exact keywords from the job description and integrates them—without inventing synonyms.
- Generates an **ATS match score (0–100)** along with a list of gaps.
- Uses a linear structure—no tables or columns (compatible with Workday, SAP, Greenhouse, Lever, and Taleo).
- Presents quantified achievements using the formula: verb + task + context + result.
- Adapts the tone based on professional level: junior, mid-level, senior, or executive.
- Includes a changelog (for Mode B).
- Provides a keyword map: shows which terms from the job description appear in which section of the resume.

## How to use it

1. Copy the content of `skill.md` (or your preferred prompt).
2. Paste it as the first message in your LLM (ChatGPT, Claude, etc.).
3. Provide the required inputs:
- Your personal details, experience, and education.
- The full text of the job description.
- (For Mode B) Upload your current resume.
4. Receive your optimized resume, match score, and recommendations.

## Key Rules to Follow

| Rule | Why |
|-------|---------|
| Exact keywords, not synonyms | ATS systems compare text strings |
| Standard sections | The parser looks for specific headings |
| Single-column layout, no tables | Prevents the parser from missing content |
| Quantifiable achievements | Distinguishes "responsible for" from "increased by 30%" |
| No information in headers/footers | Many ATS systems do not read these areas |
| Flawless spelling | A typo = a lost keyword |

## License

MIT
