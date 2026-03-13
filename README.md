# Malaysia Resume Creator

A free, browser-based resume builder designed specifically for the **Malaysian job market** — following HR-recommended standards from platforms like Jobstreet, Maukerja, and ResumeWriter.my.

> No sign-up. No data stored. Everything runs in your browser.

---

## Live Demo

[Open Malaysia Resume Creator](https://trulypureman.github.io/malaysia-resume-creator)

---

## What's New in v2

| Feature | Details |
| --- | --- |
| PDF Export (jsPDF) | Real PDF generation via jsPDF + html2canvas — no more print dialog |
| Template Toggle | Switch between **Corporate Classic** and **Modern Minimal** layouts |
| Drag-and-Drop Reorder | Grab the handle on any section and drag it to reorder your resume structure |

---

## Features

- **Malaysian HR Standard** — Sections and field order follow what local recruiters expect
- **Fill-in-the-blank Form** — No design skills needed; just fill and generate
- **Live Preview** — See your formatted resume before downloading
- **Two Resume Templates** — Corporate Classic (traditional) or Modern Minimal (sidebar layout)
- **Download as PDF** — Real PDF file generated client-side via jsPDF
- **Export as .docx** — Real Word document, ready to upload to Google Drive and open in Google Docs
- **Drag-and-Drop Section Reorder** — Customise the order sections appear in your resume
- **ATS-Friendly** — Skills section structured to pass Applicant Tracking Systems
- **Privacy First** — Zero data sent to any server; all processing is local

---

## Resume Sections Included

| Section | Status | Notes |
| --- | --- | --- |
| Personal Information | Required | Name, contact, NRIC, nationality, gender, race, marital status |
| Professional Summary | Required | 3–5 sentence elevator pitch |
| Work Experience | Required | Position, company, date range, achievements |
| Education | Required | Degree, institution, CGPA |
| Key Skills | Required | Hard skills and soft skills, tag-based and ATS-optimised |
| Languages | Optional | With proficiency level — important in the Malaysian market |
| Certifications & Training | Optional | HRDF, Google, CIDB, online certifications |
| Awards & Achievements | Optional | Academic and professional recognition |
| Volunteer & Co-Curriculum | Optional | Clubs, societies, community service |
| Expected Salary & Availability | Optional | Notice period and relocation preference |
| References | Optional | Auto-fills "Available upon request" if left blank |

All sections support drag-and-drop reordering.

---

## Templates

### Corporate Classic
Traditional layout with a navy header underline and gold section dividers. Best for formal industries — finance, government, engineering.

### Modern Minimal
Two-column layout with a dark navy sidebar (contact, skills, languages) and a clean white main column. Best for creative, tech, and business roles.

---

## How to Export to Google Docs

1. Fill in your resume details
2. Click **Export .docx**
3. Open [Google Drive](https://drive.google.com) and upload the downloaded `.docx` file
4. Right-click the file and select **Open with Google Docs**

---

## Tech Stack

| Technology | Purpose |
| --- | --- |
| HTML / CSS / JavaScript | Core application — single file, zero dependencies |
| [docx.js](https://docx.js.org/) via CDN | Generates real `.docx` Word files client-side |
| [jsPDF](https://github.com/parallax/jsPDF) via CDN | Generates real `.pdf` files client-side |
| [html2canvas](https://html2canvas.hertzen.com/) via CDN | Renders resume HTML to canvas for PDF capture |
| Google Fonts | Typography (DM Serif Display, DM Sans) |

No frameworks. No build tools. No backend. The entire application is contained in a single `index.html` file.

---

## Project Structure

```
malaysia-resume-creator/
│
├── index.html       # The entire application (single file)
└── README.md        # This file
```

---

## Contributing

Suggestions and improvements are welcome.

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push and open a Pull Request

---

## Disclaimer

This is a personal fun project built for learning and convenience purposes only. It is not intended for commercialisation, monetary gain, or any form of business use. All resume data is processed entirely in your browser — nothing is stored or transmitted to any server.

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

Created by **AhChai** with Love
