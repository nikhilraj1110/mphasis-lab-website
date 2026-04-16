# Content Audit Protocol

## Trigger
When the user points to this file and names a section on any webpage, execute the following workflow.

## Purpose
Systematically find missing or additional information that should be included in a specific section of the website. Every finding must be source-backed — no assumptions, no fabrication.

## Data Sources (in priority order)

### 1. Source Folder (READ-ONLY)
- **Path:** `/Users/raj/Desktop/projects/Workspace/Source/`
- Contains: Reports, proposals, emails, documents, images across all fiscal years
- Key subfolders: `FY 2025-2026/`, `FY 2024-2025/`, `FY 2023-2024/` and earlier
- Search thoroughly across ALL years, not just the current FY

### 2. Thunderbird Inbox (READ-ONLY)
- **Path:** `/Users/raj/Library/Thunderbird/Profiles/nbrlg44p.default-release/ImapMail/imap.gmail.com/`
- Contains: All work emails (nikhil.raj@ashoka.edu.in) in mbox format
- Key folders: `INBOX`, `[Gmail].sbd/` (Sent Mail, All Mail, Drafts), custom labels
- Search for emails related to the section topic — announcements, updates, achievements, partnerships, etc.

### 3. Annual Review Materials (READ-ONLY)
- **Fact Sheets:** `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/`
- **Comprehensive Report:** `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Comprehensive Report/`
- Contains: Per-project verified data (23 projects), aggregated metrics, publications, collaborations

### 4. Knowledge Graph Index (READ-ONLY)
- **Path:** `/Users/raj/Desktop/projects/Workspace/Knowledge-Graph-Task/.claude_index/`
- Contains: Entity relationships, people, projects, summaries
- Use as a starting point, but always verify against original Source files

### 5. Google Drive (READ-ONLY)
- **Work:** `/Users/raj/Library/CloudStorage/GoogleDrive-nikhil.raj@ashoka.edu.in/`
- **Personal:** `/Users/raj/Library/CloudStorage/GoogleDrive-nikhilraj.nr9899@gmail.com/`
- Contains: PDFs, DOCX, XLSX, images, .eml files
- Note: Native Google formats (.gdoc, .gsheet) are shortcut links only — not readable locally

### 6. The Website Itself
- **Path:** `/Users/raj/Desktop/projects/Work/Workspace/Website/`
- Cross-reference data files: `src/data/projects.js`, `src/data/people.js`, `src/data/publications.js`, `src/data/pillars.js`
- Check all other pages for information that might be relevant to the target section but is currently only mentioned elsewhere

## Workflow

### Step 1 — Understand the Target
- Read the section the user pointed to (HTML + data files)
- Understand exactly what information is currently displayed
- Note the content type: metrics, names, descriptions, links, dates, achievements, etc.

### Step 2 — Deep Search
Run parallel searches across all data sources:

**a) Source Folder Scan**
- Search across ALL fiscal years, not just current
- Look in quarterly reports, project reports, proposals, presentations
- Check for achievements, metrics, names, events, dates that relate to the section
- Pay attention to appendices, annexures, and attachments — they often contain data not in the main body

**b) Email Scan**
- Search the Thunderbird INBOX mbox file for keywords related to the section
- Look for announcements, confirmations, updates, congratulatory emails
- Check for forwarded press coverage, event confirmations, partnership agreements
- Extract dates, names, specifics from email threads

**c) Annual Review Cross-Reference**
- Check every project fact sheet for information relevant to the section
- Cross-reference the Comprehensive Report's appendices
- Look for data that was verified for the Annual Review but not yet on the website

**d) Website Cross-Reference**
- Check ALL pages of the website for related information
- Look for inconsistencies (e.g., a metric on the homepage that differs from the impact page)
- Check if information mentioned in one section should also appear in the target section

### Step 3 — Flag Findings
Present each finding as a structured question using AskUserQuestion:

**Format for each finding:**
```
FINDING: [What was found]
SOURCE: [Exact file path, email subject/date, or page:line reference]
CURRENTLY ON WEBSITE: [Yes/No — and where, if yes]
RECOMMENDATION: [Add / Update / Verify with user]
RELEVANCE: [Why this belongs in the target section]
```

**Rules for findings:**
- Every finding MUST have a verifiable source — no assumptions
- If a source is ambiguous or unclear, flag it as "NEEDS VERIFICATION"
- Do not present information you are not confident about
- Present findings one by one, not all at once
- Wait for user approval/rejection before proceeding to next finding
- Group related findings together when it makes sense

### Step 4 — Implement Approved Changes
- Only after the user approves each finding
- Make changes to the website section
- Verify the change renders correctly
- Move to the next finding

## What to Look For (by section type)

### For "Deployed Systems" / Project sections:
- New systems deployed since last update
- Updated metrics or reach for existing systems
- New partnerships or users
- Media coverage or awards related to the system
- Student contributions not yet credited

### For "Awards & Recognition":
- Awards, honors, fellowships not yet listed
- Conference best paper awards
- Media features and press coverage
- Government recognition or policy citations
- Student competition wins

### For "Publications":
- Papers published but not yet on the website
- Preprints that have been accepted
- DOI links missing from existing entries
- Workshop papers or presentations
- Book chapters or invited contributions

### For "People":
- New team members not yet added
- Role changes or promotions
- Alumni updates (new positions, further studies)
- Visiting researchers or collaborators

### For "Impact" / Metrics:
- Updated numbers (publications count, partnerships, etc.)
- New beneficiary data
- Student outcome updates
- Community engagement metrics
- K-12 outreach numbers

### For "News & Events":
- Events that happened but aren't listed
- Upcoming events confirmed via email
- Media coverage not yet linked
- Workshop/hackathon outcomes

## Rules
- **NEVER write to Source/, Thunderbird, or Google Drive folders**
- **Every finding must be source-backed — no fabrication, no assumptions**
- **Flag uncertainties explicitly — "this might be X but needs verification"**
- **Be thorough — check across ALL years, not just current FY**
- **Cross-reference across sources — if an email mentions an award, check if it's in the fact sheets too**
- **Present findings in order of confidence (highest confidence first)**
- **Do not overwhelm — if there are 20+ findings, batch them into logical groups**
