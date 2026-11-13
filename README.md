# Malaysia Resume Creator

A free, browser-based resume builder for the **Malaysian job market**. It produces ATS-friendly resumes, checks them with a live ATS health score and matches them against a job description.

> No sign-up. Nothing uploaded. Everything runs in your browser.

---

## Live Demo

[Open Malaysia Resume Creator](https://trulypureman.github.io/malaysia-resume-creator)

---

## What's New in v3

| Area | Change |
| --- | --- |
| **Real text PDF** | The PDF is now built with real, selectable text via jsPDF. v2 exported a *screenshot*, which applicant tracking systems (ATS) cannot read. |
| **ATS-safe templates** | Classic and Modern are both single-column. The v2 two-column sidebar was removed because ATS parsers often scramble columns. |
| **ATS Health Score** | Live 0–100 score with fix-it tips: contact details, summary length, quantified bullets, weak openers ("Responsible for…"), skills count, date consistency, length and personal-data exposure. |
| **Job Description Match** | Paste a JobStreet, LinkedIn, Hiredly or MauKerja ad to see matched and missing keywords. Tap a missing one to add it to your skills. |
| **Section order works** | Drag (⠿) or use ↑ ↓ and the exported resume follows the same order. In v2, reordering didn't affect the output. Includes *Experienced* and *Fresh graduate* presets. |
| **Auto-save & backup** | Data auto-saves to your browser's localStorage. Backup and Restore it as JSON to move between devices. |
| **Better Word export** | Real Word headings, native bullets, right-aligned dates on a tab stop and A4 page size. |
| **Plain-text copy** | One click copies an ATS-clean text version for online application forms. |
| **Projects section** | Built for fresh grads and tech roles: final year project, side projects, freelance work. |
| **Privacy by default** | NRIC, DOB, race, gender and marital status are hidden unless you switch them on. |
| **Auto-fit PDF** | If only a few lines spill onto the next page, spacing tightens automatically. Font sizes stay the same. |
| **Hardening** | All user input is HTML-escaped, entries can be reordered, and the app works on mobile. |

---

## Why These Choices (ATS Rules Applied)

- **Single column, no tables, no text boxes, no images.** Parsers such as Workday, SAP SuccessFactors, Taleo and Greenhouse read top-to-bottom text most reliably.
- **Standard headings:** "Professional Summary", "Skills", "Work Experience", "Education" and "Certifications". These map cleanly to ATS fields.
- **Standard fonts:** Times/Helvetica in the PDF, Georgia/Calibri/Arial in Word.
- **Contact details in the body**, not in a header or footer, which some parsers skip.
- **Dates as `Mon YYYY – Mon YYYY`** on the same line as the job title.
- **Skills as plain comma-separated text**, not graphics or rating bars.

---

## Resume Sections

| Section | Default | Notes |
| --- | --- | --- |
| Contact Details | Core | Name, target job title, email, phone, location, LinkedIn, portfolio |
| Personal Particulars | Off | NRIC, DOB, gender, race, marital status, nationality. Shown only if you turn them on |
| Professional Summary | Core | 40–100 words |
| Skills | Core | Hard skills/tools and soft skills |
| Work Experience | Core | Employment type, dates, achievement bullets |
| Projects | Optional | Strong for fresh grads and tech roles |
| Education | Core | Covers PhD to SPM, plus UEC, STPM, Matriculation and SKM |
| Certifications | Optional | Professional certs, HRD Corp courses, licences |
| Languages | Optional | Proficiency plus proof (MUET, IELTS, HSK) |
| Awards & Achievements | Optional | |
| Leadership & Activities | Optional | Co-curricular, clubs, volunteering |
| Additional Information | Optional | Expected/current salary, notice period, relocation, driving licence |
| References | Optional | "Available upon request" line is opt-in |

---

## Known Limitation

The PDF uses the standard built-in PDF fonts, which support Latin characters only. If your resume contains Chinese, Tamil or Jawi script, the app warns you and drops those characters from the PDF. Use the **Word (.docx)** export to keep them.

---

## How to Export to Google Docs

1. Click **Word (.docx)**
2. Upload the file to [Google Drive](https://drive.google.com)
3. Right-click it and choose **Open with › Google Docs**

---

## Tech Stack

| Technology | Purpose |
| --- | --- |
| HTML / CSS / JavaScript | The whole app lives in a single file. No framework, no build step |
| [jsPDF](https://github.com/parallax/jsPDF) 2.5.1 (CDN) | Text-based PDF generation |
| [docx](https://docx.js.org/) 8.5.0 (CDN) | Native Word document generation |
| Google Fonts | UI typography (DM Serif Display, DM Sans) |

Architecture: the form state is turned into a single **resume model**. Four renderers (HTML preview, PDF, DOCX, plain text) draw from that model, so every output always contains the same content in the same order.

---

## Project Structure

```
malaysia-resume-creator/
├── index.html   # The entire application
├── README.md
└── LICENSE
```

---

## Contributing

Suggestions and improvements are welcome.

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit: `git commit -m "Add your feature"`
4. Push and open a Pull Request

---

## Disclaimer

This is a personal fun project built for learning and convenience only. It is not intended for commercialisation, monetary gain or any business use. The ATS score is guidance, not a guarantee, because every employer configures its ATS differently. All resume data is processed in your browser and stored only in your browser's localStorage.

---

## License

Open source under the [MIT License](LICENSE).

---

Created by **AhChai** with Love
