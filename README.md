# Phishing Email Detection System

**IBM SkillsBuild Cyber Security BootCamp 2026 — Beginner Project**  
**Author:** Mohd Danish Ali

## Project description
A beginner-friendly Python program that reviews email subject/body text and optional sender/attachment details for common phishing warning signs. It uses explainable, rule-based checks and returns an illustrative risk score, a classification, and the indicators that triggered the score.

This is an educational prototype. It does not prove that an email is safe and must not replace approved organizational security tools or human review.

## Features
- Flags urgent or threatening wording.
- Detects requests for passwords, OTPs, and financial details.
- Checks for URL shorteners, IP-address-based links, and non-HTTPS links.
- Flags selected potentially risky attachment extensions.
- Performs a basic sender display-name/domain consistency check.
- Explains which indicators contributed to the result.

## Technologies used
- Python 3.10+
- Jupyter Notebook (`.ipynb`)
- Python standard library: `re`, `urllib.parse`, and `collections`

No third-party libraries are required.

## Dataset
The notebook includes fictional demonstration examples, so it runs without an external dataset.

Optional related learning dataset:
- [UCI Spambase](https://archive.ics.uci.edu/dataset/94/spambase) — a general email spam dataset. It is **not** a dedicated phishing-labeled dataset and is not required to run this project.

## Setup and run instructions
1. Install Python 3.10 or later.
2. Install Jupyter Notebook/JupyterLab if it is not already available in your environment.
3. Download or open `MohdDanishAli_PhishingEmailDetectionSystem.ipynb`.
4. Start Jupyter and open the notebook.
5. Run all cells from top to bottom.

The detector code itself uses only the Python standard library. Jupyter is needed only to open and run the notebook interactively.

## Understanding the output
- **LOWER RISK:** No strong configured indicators were found.
- **CAUTION:** Some warning indicators were found; review carefully.
- **HIGH RISK:** Multiple or stronger indicators were found.

The score is a simple demonstration score, not a probability. A low score does not guarantee safety.

## Responsible use and limitations
- Use only fictional, public training, or otherwise authorized email text.
- Never paste passwords, OTPs, private messages, or confidential organizational data into the notebook.
- Do not open suspicious links or attachments to test them.
- The prototype does not inspect full email headers, verify sender authentication, scan attachments, visit links, or query threat-intelligence services.
- False positives and false negatives are possible. Report suspicious emails through your institution's approved process.

## Project files
- `MohdDanishAli_PhishingEmailDetectionSystem.ipynb` — complete project code and demonstrations.
- `requirements.txt` — dependency information.
- `MohdDanishAli_ProjectReport.docx` — project report.
- `README.md` — project overview and run instructions.
