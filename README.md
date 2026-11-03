# Types of SQL Injection: IT Capstone Project

Boston Institute of Analytics, Professional Certification in Cybersecurity and Ethical Hacking (2026).

## Overview
A research and proof-of-concept project on SQL injection (SQLi): how each type works, what causes it, how much damage it can do, and how to prevent it.

## What's covered
- **Types researched:** in-band (error-based and union-based), blind (boolean-based and time-based) and out-of-band SQL injection, including causes and impact.
- **Proof of concept:** a union-based SQL injection on a PortSwigger Web Security Academy lab.
  - Confirmed the flaw by adding a single quote.
  - Found the 2-column query with `ORDER BY`.
  - Checked column types with `UNION SELECT NULL`.
  - Extracted usernames and passwords from the users table with `UNION SELECT` and logged in as the administrator to solve the lab.
- **Reconnaissance:** profiled the target's technology stack with Wappalyzer and wrote an impact analysis.
- **Recommendations:** parameterized queries, least-privilege database accounts, input validation, hiding verbose errors, a WAF, password hashing and regular testing.

## Repository contents
| Item | Description |
| --- | --- |
| `IT Capstone Project Topic Types of SQL Injection.docx` | Full written report |
| `IT Capstone Types of SQL Injection.pptx` | Presentation slides |
| `Code and Tools for IT Capstone Project.txt` | Tools and example payloads used |
| `Scrrenshots for POC/` | Screenshots of the lab walkthrough |

## Tools
Google Chrome, Wappalyzer, PortSwigger Web Security Academy.

## Disclaimer
All testing was done in an intentionally vulnerable lab built for training. Do not test systems you do not own or have written permission to test.
