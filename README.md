# Sumeru Health Sciences — Academic Medical Center & Health System

> **A premium, responsive clinical dashboard and public hospital landing page engineered with evidence-based healthcare UX principles.**

This repository contains the digital experience platform for **Sumeru Health Sciences**, an academic medical center integrating quaternary surgical care, multidisciplinary clinical institutes, translational research, and patient-first care delivery.

---

## Architecture Overview

The project provides two complementary, interconnected web applications:

1. **Public Institutional Landing Page (`landing.html`)**
   - **Hero Composition**: Balanced editorial 12-column layout pairing academic mission narrative with an active Clinical Faculty Spotlight card (Dr. Helena Vance, MD).
   - **Hub-and-Spoke Triage Matrix**: Rapid access tiles for finding specialists, scheduling visits, exploring institutes, opening MyChart, and reaching the 24/7 nurse hotline.
   - **Clinical Centers of Excellence**: Dedicated specialty cards covering Cardiovascular & Thoracic Sciences, Comprehensive Oncology, Neurological Sciences, Orthopedics, Digestive Health, and Maternal & Fetal Medicine.
   - **Distinguished Faculty**: Profile cards detailing board credentials, clinical pavilions, and outpatient clinic hours.
   - **Modern Facilities & Wayfinding**: In-depth overviews of Hybrid Robotic Operating Suites, 3T MRI & CAP/CLIA Core Labs, and Private Inpatient Healing Suites.
   - **Interactive Consultation Booking**: Complete request form with required field validation, immediate receipt generation (`#modal-confirmation`), and SMS/telephone triage confirmation workflows.

2. **Authenticated Patient Dashboard Portal (`index.html`)**
   - **Unified Single-Scroll Experience**: Responsive navigation designed according to `DESIGN.md` specifications.
   - **Comprehensive Views**:
     - **Home**: Real-time care alerts, vital sign telemetry summaries, next appointment cards, and recent lab results.
     - **My Health Records**: Clinical history, past surgical reports, immunization records, and allergy profiles.
     - **Appointments**: Upcoming surgical follow-ups, calendar integrations, and doctor booking wizards.
     - **Care & Test Results**: Tabular lab panels (CBC, Lipid Panel, Metabolic Panels) with reference ranges and physician notes.
     - **Billing & Insurance**: Coverage status, copay ledger, deductible tracking, and statement downloads.
     - **Hospital & Campus Operations**: Interactive floor maps, visitor guidelines, transit options, and dining schedules.

3. **Design System & Authoritative Specification**
   - [`DESIGN.md`](./DESIGN.md): The comprehensive 534-line foundational design document detailing brand identity, color theory, typography hierarchy, clinical component tokens, and UX rules.
   - [`STITCH-TOKENS.md`](./STITCH-TOKENS.md): Google Stitch design token definitions and CSS custom properties.

---

## Design System Highlights

- **Palette**: Deep Navy (`#0B1B3D`), Lumera Spruce Green (`#0F766E`), Lumera Cyan (`#0284C7`), Emergency Crimson (`#BE123C`), and clinical neutrals.
- **Typography**: 
  - *Newsreader* (Editorial Serif) for institutional headlines and hero statements.
  - *Plus Jakarta Sans* (Humanist Sans) for UI panels, navigation, and body copy.
  - *Inter* (Tabular Sans) for biometric metrics, clinical data, lab numbers, and reference codes.
- **Icons**: Clean Google Material Symbols Outlined strictly contained (`overflow: hidden; width: 1em; height: 1em`) for high clarity and zero layout shifting.

---

## Quickstart / Running Locally

The application runs on vanilla HTML5, CSS3, Tailwind CSS CDN, and native JavaScript. No compilation or heavy node build steps are required.

### Using Python:
```bash
python -m http.server 3000
```
Then navigate to:
- **Public Landing Page**: `http://localhost:3000/landing.html`
- **Patient Dashboard**: `http://localhost:3000/index.html`

### Using Node / npx:
```bash
npx serve .
```

---

## Project Structure

```text
├── assets/
│   ├── images/
│   │   └── dr-helena-vance.jpg     # Faculty portrait asset
│   └── reference-screen.png        # Design reference artifact
├── backup/
│   └── DESIGN.md.bak               # Checkpoint backup of authoritative design spec
├── DESIGN.md                       # Authoritative 534-line design system specification
├── STITCH-TOKENS.md                # Google Stitch token documentation
├── index.html                      # Patient Dashboard web application
├── landing.html                    # Public Hospital Landing Page
├── README.md                       # Repository overview and documentation
└── .gitignore                      # Git ignore rules
```

---

## Educational Prototype Notice

*Sumeru Health Sciences & Academic Medical Center is an educational UI/UX design prototype. Clinical metrics, doctor names, and patient data presented in this repository are demonstration artifacts.*
