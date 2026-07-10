# TalentFlow AI

An AI-powered recruitment platform that automates resume screening, candidate evaluation, and job-fit ranking. It combines a custom web dashboard with an n8n automation backend.

## The Problem

Manually screening resumes takes forever. Recruiters have to open every attachment, read through inconsistent formats, cross check each candidate against the job requirements, and figure out who's actually a good fit, all by hand. It doesn't scale, it's easy to miss good candidates, and every recruiter ends up judging fit differently. TalentFlow AI was built to fix that.

## The Solution

TalentFlow AI takes the manual work out of the process. Resumes come in through email and get pulled automatically, no downloading or sorting by hand. AI reads each resume, pulls out the candidate's details, and scores them against the job description using the same criteria every time. Recruiters get a single dashboard showing every applicant, their fit rating, and a ranked shortlist for any client's requirements, so they can spend their time actually talking to good candidates instead of digging through inboxes.

## What It Does

- **Automatic resume intake** so applicant emails and attachments (PDF/DOCX) are picked up automatically, no manual downloading or sorting.
- **AI-powered parsing** that extracts candidate name, email, contact number, and resume content into structured data.
- **Job-fit scoring** where each applicant is evaluated against a job description, producing strengths, weaknesses, risk/reward factors, and an overall fit rating.
- **Client resource matching** so you can post a role's budget and requirements and get back a ranked shortlist of the best-fit candidates.
- **Centralized dashboard** showing total applicants, average fit rating, and roles represented at a glance, with full candidate details one click away.

## App Screens

- **AI Resume Analyzer** dashboard view of all applicants with location, salary expectations, and fit ratings
- **Create Job Opening** a 3 step flow (Position, Details, Results) to post a role, set budget/country, and get matched applicants
- **Job Descriptions** write or update the JD used to score candidates for a given position

## How It Works

1. Resumes arrive via email and get parsed (PDF and DOCX supported).
2. Cohere AI extracts candidate details and evaluates fit against the job description.
3. Results are stored and served back to the web app, powering the dashboard and ranked shortlists.

## Tech Stack

- **Frontend:** ReactJS, React Router
- **Automation:** n8n (workflow orchestration)
- **Backend:** Python
- **AI:** Cohere (resume parsing and candidate evaluation)
- **Data:** Google Sheets (candidate records), Google Drive (file handling)
- **Ingestion:** Gmail Trigger / IMAP

## Outcome

Turns resume screening from a manual, hours long process into an instant, AI scored shortlist, giving recruiters a single dashboard to post roles, review applicants, and find the best fit candidates for any client requirement.
