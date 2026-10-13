# PS-013 — Incident Timeline and Evidence Collection for Small Teams

## Project Overview
This project aims to help small cybersecurity teams process authorized log files, preserve evidence integrity, normalize timestamps, and reconstruct a searchable incident timeline.

## Problem Statement
AIORI 3 Hackathon — PS-013: Incident Timeline and Evidence Collection for Small Teams.

## Objectives
- Process at least two different text-log formats.
- Preserve original log records.
- Calculate SHA-256 hashes for collected files.
- Normalize timestamps to UTC where sufficient information is available.
- Document timestamp uncertainty and parsing gaps.
- Create a searchable chronological timeline.
- Export an incident summary.
- Test three synthetic scenarios.
- Compare manual and tool-assisted triage time.

## Proposed Workflow
Log ingestion → Evidence hashing → Parsing → Timestamp normalization → Timeline generation → Search and report → Evaluation.

## Technology Stack
- Python
- hashlib, re, datetime, zoneinfo, csv and json
- pytest or unittest, if used
- SQLite or Streamlit, if implemented

## Test Scenarios
1. Web access-log scenario.
2. Linux syslog-style service-event scenario.
3. Mixed timestamp, simulated clock-skew and malformed-record scenario.

## Installation and Usage
Document the tested Python version, dependencies, setup commands, and the actual command used to run the application.

## Testing and Evaluation
Publish actual results for hash verification, event coverage, timestamp ordering, parsing gaps and triage time. Do not invent results.

## Limitations
Document unsupported formats, time-zone assumptions, clock-skew limitations and the need for analyst review.

## Team Contributions
List each member's actual implementation, testing, design and documentation responsibilities.

## Responsible Use
Use synthetic or authorized logs. Do not publish credentials, personal information or confidential incident evidence.

## References
NIST SP 800-86 — Guide to Integrating Forensic Techniques into Incident Response:
https://csrc.nist.gov/pubs/sp/800/86/final
