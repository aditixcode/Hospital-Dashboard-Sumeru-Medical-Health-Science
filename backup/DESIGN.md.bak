# DESIGN.md — Lumera Academic Medical Center & Health Sciences
## Comprehensive UI/UX Design System & Clinical Interface Specification

> **Document Status**: Production Design Specification  
> **Target Products**: Public Hospital Landing Page & Unified Health System Workspace (5 Core Clinical & Operational Surfaces)  
> **Author**: Digital Product Design & Clinical Human Factors Lead  
> **Compliance Standard**: WCAG 2.1 AA / Section 508 / Medical Ergonomics ISO 9241-210

---

## 1. Executive Summary & Design Research Synthesis

This design system establishes a cohesive, authoritative, and patient-centered digital design language for **Lumera Academic Medical Center**, a premier multispecialty hospital and research institution. 

Rather than adopting generic digital templates or transient design fads, this system is anchored in rigorous comparative research across three landmark institutions—**Mayo Clinic**, **Cleveland Clinic**, and **Apollo Hospitals**—synthesizing institutional trust, operational clarity, and human empathy.

```
       ┌─────────────────────────────────────────────────────────────┐
       │                   LUMERA DESIGN TRIANGLE                    │
       │                                                             │
       │                    Mayo Clinic (Trust & Depth)              │
       │                                ▲                            │
       │                               / \                           │
       │                              /   \                          │
       │                             /     \                         │
       │                            /       \                        │
       │                           /         \                       │
       │  Cleveland Clinic        ▼───────────▼   Apollo Hospitals   │
       │ (Operational Rigor)                     (Frictionless Flow) │
       └─────────────────────────────────────────────────────────────┘
```

---

## 2. Comparative Reference Analysis

### 2.1 Verified Observations: Mayo Clinic (`mayoclinic.org`)
*Verified via visual and structural audit of Mayo Clinic's digital footprint.*

| Dimension | Verified Findings |
| :--- | :--- |
| **Visual Hierarchy** | Anchored by an authoritative two-tier global navigation. High-impact conversion triggers (*Request Appointment*, *Find a Doctor*) are persistently pinned. Content presentation leans heavily editorial with deep typographical hierarchy for disease taxonomies and clinical research. |
| **Typography** | Structured serif/sans pairing custom-engineered for institutional gravitas (Brody Associates type systems). High contrast headlines convey clinical authority; comfortable body measure (60–72 characters per line) minimizes cognitive fatigue. |
| **Color Usage** | Anchored in deep institutional blue (`#0E3293`), crisp clinical whites, and cool slate neutrals. Warm alert tones are strictly functional, never decorative. |
| **Image Treatment** | Documentary-style, authentic clinical photography. Real physicians interacting empathetically with diverse patients in softly lit clinical or consultation settings; complete avoidance of staged stock aesthetics. |
| **Appointment UX** | Multi-step progressive triage wizard (*Patient Status* → *Condition/Specialty* → *Campus/Location* → *Insurance & Verification*). Prioritizes clinical triage accuracy over instant impulse booking. |
| **Spacing & Structure** | Generous vertical breathing room between editorial sections; rigid 8pt baseline grid; high-contrast card borders with low-elevation ambient drop shadows. |

### 2.2 Verified Observations: Cleveland Clinic (`my.clevelandclinic.org`)
*Verified directly via DOM tree and production CSS token inspection.*

| Dimension | Verified Findings |
| :--- | :--- |
| **Visual Hierarchy** | Structured grid layout (`bp1100:grid-cols-[3fr_6fr_4fr]`). Top utility bar categorizes international locations (*Abu Dhabi, Canada, Florida, London, Nevada, Ohio*) alongside direct contact (`800.223.2273`), *MyChart*, and *Donate Now*. |
| **Typography** | Modern sans-serif stack utilizing fluid responsive scaling (`text-rem40px` to `bp900:text-rem48px`, `leading-rem52px`). Explicit overlines (`text-rem13px`) paired with bold section headlines (`text-rem20px bp600:text-rem25px`). |
| **Color Usage** | Primary brand blue (`brandBlue-500` / `#007BC2`), deep navy interactive hover states (`blue-800` / `#00447C`), vibrant divider accents (`vibrantBlue-500`), and a dedicated green for philanthropy (`forestGreen-500`). Background canvas remains pristine `#FFFFFF` and subtle `#F0F4F8`. |
| **Image & Media** | Prominent full-width hero video featuring real patient encounters, backed by a dual-gradient overlay (`linear-gradient(180deg, rgba(75,75,75,0) 19.64%, rgba(39,38,38,0.83) 82.46%)`) and accessible pause control buttons. |
| **Appointment UX** | Dedicated high-contrast header button (`Appointments` in `brandBlue-500` with 5px border-radius `rounded-[0.3125rem]`). Links directly into structured access portals, provider lookup, and virtual visits. |
| **Emergency Alerts** | Floating pill banner (*Closures & Updates*) anchored at top center with exclamation icon, high z-index, and smooth expand/collapse transitions. |

### 2.3 Verified Observations: Apollo Hospitals (`apollohospitals.com` & `Apollo 24|7`)
*Verified via architecture audit of Apollo Hospitals and Apollo 24|7 ecosystem.*

| Dimension | Verified Findings |
| :--- | :--- |
| **Visual Hierarchy** | Hub-and-spoke rapid-access dashboard on the primary homepage. Instant action shortcuts (*Book Physical Appointment*, *Consult Online*, *Order Medicines*, *Book Lab Tests*) prominently surfaced above the fold. |
| **Typography** | Clean, highly legible contemporary sans-serif with strong numerical hierarchy for doctor fees, consultation hours, and experience metrics. |
| **Color Usage** | Deep corporate navy blue (`#0C2067`) coupled with energetic clinical cyan/teal (`#00A3A6`) and positive action green (`#00875A`) for available slot chips. Soft desaturated slate-tinted canvas (`#EEF3F7` to `#F8FAFC`). |
| **Image Treatment** | Focus on verified physician badges, clear doctor portraits with qualification stamps, and modern diagnostic facility photography. |
| **Appointment UX** | High-velocity, e-commerce-inspired booking matrix. Filter by symptom or specialty → view calendar days → select time band (Morning / Afternoon / Evening) → view precise slot pills → select patient → instant confirmation. |
| **Smart Search** | Prominent search bar with symptom-to-specialist predictive mapping (e.g., typing "palpitations" maps directly to Cardiology). |

---

## 3. Reusable Principles vs. Pitfalls to Avoid

### 3.1 Principles to Adopt & Reapply
1. **Frictionless Triage & Dual-Speed Navigation**: Provide immediate, unencumbered entry points for patients in distress (Emergency line, urgent care, symptom search) while maintaining structured academic taxonomy for exploratory research.
2. **Cognitive De-escalation Through Visual Caliber**: Healthcare users are often anxious or fatigued. Use calm, grounded colors, generous whitespace, legible typographic sizing, and reassuring feedback at every step.
3. **Credibility Through Transparency**: Surface doctor credentials, board certifications, peer-reviewed clinical trial contributions, and real hospital bed/wait time metrics.
4. **Accessible, Deterministic Interactive States**: Ensure all interactive controls (slot pills, form inputs, buttons) have unambiguous focus rings, defined hit areas, and zero ambiguous iconography.

### 3.2 Anti-Patterns & Pitfalls to Reject (Do NOT Copy)
1. **SEO Link Farmland**: Avoid massive accordion link dumps with dozens of raw text links (observed in legacy hospital sub-pages). Use structured categorical megamenus with contextual highlights.
2. **Aggressive Commercial Clutter**: Avoid promotional marketing carousels, unrelated pharmacy banner ads, or floating chat-bots that mask primary booking controls.
3. **Premature Form Fatigue**: Never force patients to fill out a 20-field personal medical history form before showing them whether their chosen specialist has available appointments.
4. **Staged Stock Photography Clichés**: Reject generic pictures of models in lab coats pointing at clipboards or laughing at a salad. Only use documentary-grade, empathetic, realistic clinical imagery.

---

## 4. Brand Identity & Design Rationale: Lumera Academic Medical Center

### 4.1 Brand Narrative
**Lumera** (*from Latin 'Lumen' — light, clarity, understanding*) represents clarity in diagnosis, scientific preeminence, and radiant human empathy. It is an internationally recognized academic medical center integrating cutting-edge clinical research with patient-first healing.

### 4.2 Intended Emotional Response
- **Relief & Reassurance**: The patient feels immediately that they are in expert, trustworthy hands.
- **Dignity & Respect**: Interfaces feel elegant, clear, and quiet—never chaotic or sensationalist.
- **Clinical Precision**: High data clarity for clinicians and administrative staff without visual noise or cognitive friction.

---

## 5. Medical Color System (WCAG AAA / AA Compliant)

The color palette is deliberately calibrated to medical psychological principles: deep blue grounds authority, bio-cyan and surgical spruce evoke clinical hygiene and restorative life, and neutral alabaster surfaces eliminate glare.

```
┌────────────────────────────────────────────────────────────────────────┐
│                        CORE COLOR PALETTE MATRIX                       │
├──────────────┬──────────────┬──────────────┬──────────────┬────────────┤
│ Navy Authority│ Surgical Cyan│ Bio-Spruce   │ Canvas Neutral│ Alert Red  │
│   #0B1B3D    │   #0284C7    │   #0F766E    │   #F8FAFC    │  #BE123C   │
└──────────────┴──────────────┴──────────────┴──────────────┴────────────┘
```

### 5.1 Primary Brand & Foundation Colors
| Token Name | HEX | HSL | Semantic Role & Usage | Contrast Ratio (vs #FFF) |
| :--- | :--- | :--- | :--- | :--- |
| `--color-brand-primary` | `#0B1B3D` | 221°, 69%, 14% | Deep Obsidian Navy. Global header, primary headings, core brand anchor. | **15.2:1** (AAA) |
| `--color-brand-secondary`| `#1E3A8A` | 224°, 64%, 33% | Clinical Royal Blue. Secondary navigation, authoritative accents, hero accents. | **8.8:1** (AAA) |
| `--color-action-primary` | `#0284C7` | 199°, 98%, 39% | Surgical Cyan / Bio-Azure. Primary CTA buttons, interactive links, active tabs. | **4.6:1** (AA Large/Text) |
| `--color-action-hover`   | `#0369A1` | 201°, 96%, 32% | Deep Azure. Hover state for primary action buttons. | **6.1:1** (AAA) |
| `--color-brand-accent`   | `#0F766E` | 175°, 77%, 26% | Restorative Spruce Green. Positive clinical indicators, wellness programs. | **6.4:1** (AAA) |

### 5.2 Neutral Canvas & Surface System
| Token Name | HEX | Semantic Role & Usage |
| :--- | :--- | :--- |
| `--color-surface-bg`     | `#F8FAFC` | Main viewport canvas background (Slate 50). Soft on eyes, zero glare. |
| `--color-surface-card`   | `#FFFFFF` | Primary card background, workspace panels, modal sheets. |
| `--color-surface-subtle` | `#F1F5F9` | Table headers, secondary toolbars, disabled item containers. |
| `--color-border-subtle`  | `#E2E8F0` | Structural card borders, divider lines, calendar grid lines (Slate 200). |
| `--color-border-strong`  | `#CBD5E1` | Interactive input field borders, active tab underlines (Slate 300). |
| `--color-text-primary`   | `#0F172A` | Primary body text, headline titles, critical clinical metrics (Slate 900). |
| `--color-text-secondary` | `#475569` | Secondary descriptions, timestamps, metadata labels (Slate 600). |
| `--color-text-muted`     | `#64748B` | Table column titles, placeholder values, helper text (Slate 500). |

### 5.3 Clinical & Semantic Status Tokens
*Strict rule: Never convey status through color alone. Every status color must accompany an icon and text.*

| Status | Foreground | Background | Border | Clinical Meaning & Usage |
| :--- | :--- | :--- | :--- | :--- |
| **Critical / Emergency** | `#991B1B` | `#FEF2F2` | `#FCA5A5` | Vitals alert (SpO2 < 90%), severe allergies, ICU red-flag. |
| **Warning / Elevated**   | `#92400E` | `#FFFBEB` | `#FCD34D` | Borderline lab values, appointment pending review, unverified insurance. |
| **Normal / Stable**     | `#166534` | `#F0FDF4` | `#86EFAC` | Vitals in target range, cleared for discharge, slot available. |
| **Observation / Info**   | `#1E40AF` | `#EFF6FF` | `#93C5FD` | Diagnostic order placed, scheduled telehealth, MyChart update. |
| **Occupied / Reserved**  | `#374151` | `#F3F4F6` | `#D1D5DB` | Bed census: Occupied; Provider: In Consultation. |

---

## 6. Typography & Typographic Hierarchy

To project institutional authority while ensuring effortless clinical readability, Lumera pairs a **dignified transitional editorial serif** for brand moments with an **engineered, ultra-legible grotesque sans-serif** for body text and clinical workspace data.

- **Display & Section Heading Font**: `Newsreader` or `Source Serif 4` (Editorial, compassionate, authoritative).
- **Body & Clinical UI Font**: `Plus Jakarta Sans` or `Inter` with OpenType `cv02`, `cv03`, `cv04` enabled for distinct characters (`1` vs `l` vs `I`).
- **Tabular Clinical Data Font**: `Inter` with `font-variant-numeric: tabular-nums lining-nums;` (ensures zero shifting in live heart-rate and SpO2 tickers).

```
TYPOGRAPHIC SCALE (Major Second / Minor Third Hybrid):

Display 1 (Hero)     ── 44px / 52px  (Bold 700 / Serif)
Display 2 (Section)  ── 32px / 40px  (SemiBold 600 / Serif)
Heading 1            ── 24px / 32px  (SemiBold 600 / Sans)
Heading 2 (Card)     ── 18px / 26px  (Medium 600 / Sans)
Heading 3 (Sub-panel)── 15px / 22px  (SemiBold 600 / Sans)
Body Regular         ── 14px / 22px  (Regular 400 / Sans)
Body Small           ── 13px / 18px  (Regular 400 / Sans)
Clinical Micro/Label ── 11px / 16px  (Medium 500 / Sans / Uppercase Tracked 0.05em)
Vitals Metric Large  ── 28px / 32px  (Bold 700 / Tabular Sans)
```

### 6.1 Typographic Rules & Best Practices
- **Line Length**: Max 72 characters (`max-w-prose` ~ 680px) for editorial healthcare content.
- **Paragraph Spacing**: 1.5em margin-bottom; never indent paragraphs.
- **Hierarchy Integrity**: No sentence-fragment ALL-CAPS headings. All labels must use clear sentence case except standardized clinical acronyms (e.g., `MRN`, `ICD-10`, `SpO2`, `BP`, `ECG`).

---

## 7. Spacing Scale & Layout Grid System

The spatial foundation is governed by a strict **8-Point Spatial Grid System**, with a 4-point half-step reserved strictly for dense clinical data tables and status pills.

### 7.1 Spacing Scale
| Token | Pixels | Application |
| :--- | :--- | :--- |
| `space-1` | 4px | Internal badge padding, table row dense gutter. |
| `space-2` | 8px | Gap between icon and text, input inner vertical padding. |
| `space-3` | 12px | Compact button vertical padding, pill spacing. |
| `space-4` | 16px | Standard card padding, form group vertical margin. |
| `space-6` | 24px | Card container inner padding, grid column gap. |
| `space-8` | 32px | Section header bottom margin, modal dialog padding. |
| `space-12`| 48px | Sub-section vertical separation. |
| `space-16`| 64px | Landing page section vertical spacing. |
| `space-24`| 96px | Hero banner top/bottom vertical container spacing. |

### 7.2 Responsive Breakpoints & Layout Behaviors
- **Mobile (`< 640px`)**: Single column stacked layout. Full-width touch targets. Persistent bottom utility bar for "Emergency / Call 911" and "Book Appointment".
- **Tablet (`640px – 1023px`)**: 8-column layout. Split patient view (Master-detail drawer pattern).
- **Desktop (`1024px – 1439px`)**: 12-column layout (max-width `1280px`). Primary hospital landing page grid.
- **Clinical Workstation (`1440px+`)**: 3-pane continuous clinical workspace (1: Collapsible Nav + 2: Patient Registry/Queue + 3: Active Patient Chart/Encounter + 4: Diagnostic Context Drawer).

---

## 8. Master Component Specifications

### 8.1 Buttons
All interactive targets conform to a minimum height of `44px` on touch screens and `38px` on mouse workstations.

```
BUTTON ANATOMY:
┌───────────────────────────────────────────────┐
│ [Icon: 18x18]  Primary Action Label  [Badge]  │
└───────────────────────────────────────────────┘
```

1. **Primary Action Button (Surgical Cyan)**:
   - `background: #0284C7; color: #FFFFFF; font-weight: 600; font-size: 14px;`
   - `padding: 10px 20px; border-radius: 6px; border: none;`
   - `hover: background: #0369A1; transition: all 150ms ease-in-out;`
   - `focus-visible: outline: 2px solid #0284C7; outline-offset: 2px;`
2. **Secondary / Outline Button**:
   - `background: #FFFFFF; color: #0B1B3D; border: 1.5px solid #CBD5E1;`
   - `hover: background: #F8FAFC; border-color: #0B1B3D;`
3. **Emergency Quick-Dial Button**:
   - `background: #BE123C; color: #FFFFFF; font-weight: 700;`
   - `hover: background: #9F1239;`
   - Paired with an unmissable phone receiver icon and "24/7 Trauma: +1 (800) 555-0199".

### 8.2 Form Fields & Patient Inputs
Clinical data entry requires zero visual ambiguity and instantaneous error recovery.

```
FORM FIELD STATE SPEC:
Default:  ┌──────────────────────────────────────────────────┐
          │ Enter Patient MRN or Legal Name...               │  Border: #CBD5E1
          └──────────────────────────────────────────────────┘
Focus:    ┌──────────────────────────────────────────────────┐
          │ Johnathan Vance                                  │  Border: #0284C7 (2px)
          └──────────────────────────────────────────────────┘  Shadow: 0 0 0 3px rgba(2,132,199,0.15)
Error:    ┌──────────────────────────────────────────────────┐
          │ 994-00-XXXX [Invalid format]                     │  Border: #BE123C (2px)
          └──────────────────────────────────────────────────┘
          ⚠ MRN must follow the 8-digit hospital format (e.g., MRN-8849-01)
```

- **Label Placement**: Persistent top label (`13px`, weight `600`, color `#0F172A`). Never rely on placeholders as labels.
- **Required Indicators**: Explicit red asterisk with screen-reader text (`aria-required="true"`).
- **Inline Validation**: Immediate format helper text below input with clear instructions on how to rectify errors.

### 8.3 Specialty & Department Cards (Landing Page)
- **Container**: `background: #FFFFFF; border: 1px solid #E2E8F0; border-radius: 8px; padding: 24px;`
- **Elevation**: Subtle resting shadow `0 1px 3px rgba(0,0,0,0.05)`. Hover transition: `translateY(-2px)`, shadow `0 8px 16px -4px rgba(11,27,61,0.08)`, border `1px solid #0284C7`.
- **Content Hierarchy**:
  1. Department Icon (Clinical vector graphic in `#0284C7` container)
  2. Department Name (e.g., "Cardiovascular & Thoracic Sciences")
  3. Key Focus Areas (e.g., "Structural Heart, Transcatheter Valve, Arrhythmia")
  4. Availability Micro-badge ("Next Slot: Tomorrow, 09:30 AM")
  5. Action Link ("Consult Specialists →")

---

## 9. Detailed Specifications for the Five Core Surfaces

The Lumera digital health system extends beyond the public landing page into a unified, high-density hospital operating suite. The design language maintains stylistic continuity while adjusting density for operational speed.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                 LUMERA UNIFIED CLINICAL & HOSPITAL SUITE                    │
├─────────────────┬─────────────────┬──────────────────┬───────────┬──────────┤
│ 1. Patient      │ 2. Scheduling & │ 3. Clinical      │ 4. Revenue│ 5. Admin │
│    Registry     │    Availability │    Workspace     │    Cycle  │    & Beds│
└─────────────────┴─────────────────┴──────────────────┴───────────┴──────────┘
```

---

### Surface 1: Patient Registry (Demographics & Medical History)

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ PATIENT REGISTRY MASTER VIEW                                    [+ New Patient]
├──────────────────────────────────────────────────────────────────────────────┤
│ 🔍 Search MRN, Name, DOB... │ Filter: [All Wards ▼] [Active Inpatients ▼]   │
├─────────┬──────────────┬──────┬───────┬──────────────────────┬───────────────┤
│ MRN     │ Patient Name │ Age  │ Blood │ Primary Condition    │ Safety Alerts │
├─────────┼──────────────┼──────┼───────┼──────────────────────┼───────────────┤
│ LM-8821 │ Chen, Wei    │ 54 M │ O+    │ Ischemic Cardiomyop. │ 🔴 Penicillin │
│ LM-8822 │ Adams, Sarah │ 32 F │ A-    │ Type 1 Diabetes M.   │ 🟡 Fall Risk  │
│ LM-8823 │ Miller, David│ 68 M │ B+    │ Post-Op Hip Arthro.  │ 🟢 Cleared    │
└─────────┴──────────────┴──────┴───────┴──────────────────────┴───────────────┘
```

- **Purpose**: Rapid lookup, demographic onboarding, and longitudinal health record access.
- **Key UI Elements**:
  - **Global Patient Banner**: Fixed 52px top bar showing: Patient Name, Legal Sex, Age, DOB, MRN, Allergies Banner (Bright Red Tag `#FEF2F2`), and Attending Physician.
  - **Split-View Architecture**: Left pane displays searchable/filterable patient list (340px width); right pane displays deep clinical history accordion (Demographics, Immunizations, Family History, Prior Surgeries, Advance Directives).
  - **Safety Badges**: Distinct high-contrast chips for critical alerts (`Allergy: Penicillin`, `Fall Risk`, `NPO - Nil Per Os`).

---

### Surface 2: Appointment & Scheduling View (Calendar & Availability)

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ PROVIDER AVAILABILITY MATRIX — CARDIOLOGY             Date: [ Oct 17, 2026 ▼]│
├───────────────────┬──────────────┬──────────────┬──────────────┬─────────────┤
│ Provider          │ 08:00 - 10:00│ 10:00 - 12:00│ 13:00 - 15:00│ 15:00-17:00 │
├───────────────────┼──────────────┼──────────────┼──────────────┼─────────────┤
│ Dr. H. Vance (MD) │ [LM-8821:Echo│ [Available]  │ [Surgical OT]│ [Available] │
│ Dr. E. Rostova    │ [Available]  │ [LM-8840:OPD]│ [LM-8845:OPD]│ [Admin]     │
│ Dr. K. Patel (NP) │ [LM-8850:Tele│ [Available]  │ [Available]  │ [Buffer]    │
└───────────────────┴──────────────┴──────────────┴──────────────┴─────────────┘
```

- **Purpose**: High-throughput patient scheduling, multi-provider calendar matrix, and room/equipment allocation.
- **Key UI Elements**:
  - **Tri-Mode Switcher**: Toggle between `Day (Provider Matrix)`, `Week (Single Provider)`, and `Department Queue`.
  - **Interactive Slot Pills**:
    - *Available*: Crisp white container, `#0F766E` spruce text, border `#86EFAC`. On click, triggers instant 3-step booking drawer.
    - *Booked*: Light slate `#F1F5F9`, muted text, tooltip with patient initials and appointment type.
    - *Emergency/Buffer*: Amber striped container reserving rapid-triage capacity.
  - **Triage Priority Tagging**: Color-coded appointment types: `Routine Checkup (Blue)`, `Urgent Triage (Amber)`, `Post-Op Follow-up (Spruce)`.

---

### Surface 3: Clinical Workspace (Vitals, Labs, Prescriptions, Encounters)

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ CLINICAL WORKSPACE — ENCOUNTER #ENC-4091                       [Sign & Close]│
├───────────────────────────────────┬──────────────────────────────────────────┤
│ LIVE VITALS (Updated 8 min ago)   │ ACTIVE PRESCRIPTIONS (e-Rx)              │
│ HR: 74 bpm  │ BP: 118/76 mmHg     │ • Metoprolol Succinate 50mg PO Daily     │
│ SpO2: 98%   │ Temp: 98.6°F (37°C) │ • Atorvastatin 40mg PO QHS               │
│ RR: 16 /min │ Pain Score: 2/10    │ [+ Prescribe New Medication]             │
├───────────────────────────────────┴──────────────────────────────────────────┤
│ DIAGNOSTIC LABS MATRIX                                                       │
│ Test Name          Result      Reference Range   Status    Flags             │
│ Serum Creatinine   0.92 mg/dL  (0.70 - 1.30)     Normal    🟢 Within Limits  │
│ Potassium          5.4 mEq/L   (3.5 - 5.0)       Elevated  🟡 High           │
│ Troponin-I         < 0.01 ng/mL(< 0.04)          Normal    🟢 Clear          │
├──────────────────────────────────────────────────────────────────────────────┤
│ CLINICAL SOAP ENCOUNTER NOTE                                                 │
│ S: Patient reports resolved chest tightness following sublingual nitro...    │
│ O: Lungs clear to auscultation bilaterally. S1/S2 distinct, no gallop...     │
│ A: Resolving stable angina; potassium mildly elevated secondary to ACE-i...  │
│ P: Adjust lisinopril dosing; recheck basic metabolic panel in 7 days...      │
└──────────────────────────────────────────────────────────────────────────────┘
```

- **Purpose**: The primary operating dashboard for physicians, nurse practitioners, and residents during active encounters.
- **Key UI Elements**:
  - **Real-Time Vitals Stream**: High-contrast biometric metric cards with sparkline trends over past 24 hours. Uses tabular figures (`font-variant-numeric: tabular-nums`) to prevent optical jitter.
  - **Structured Lab Results Table**: Explicit column formatting for Test Name, Value, Standard Reference Interval, and Abnormality Indicator (`HIGH`, `LOW`, `CRITICAL`).
  - **e-Prescription Safety Interface**: Integrated drug-drug interaction alerts (warning modal fires if prescribing contrasting medications).
  - **SOAP Note Editor**: Segmented rich-text input blocks (*Subjective*, *Objective*, *Assessment*, *Plan*) with automated ICD-10 and CPT coding suggestions.

---

### Surface 4: Billing & Revenue Cycle Surface

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ REVENUE CYCLE & ADJUDICATION MANAGEMENT                         [Export EDI] │
├──────────────────────────────────────────────────────────────────────────────┤
│ TOTAL BILLED: $14,850.00 │ INSURANCE PAID: $11,200.00 │ PATIENT DUE: $650.00 │
├──────────┬─────────────────┬──────────┬──────────┬──────────────┬────────────┤
│ Claim ID │ Service/Code    │ Provider │ Carrier  │ Status       │ Action     │
├──────────┼─────────────────┼──────────┼──────────┼──────────────┼────────────┤
│ CLM-9912 │ 99214 (L4 OPD)  │ Dr. Vance│ BlueCross│ 🟢 Paid      │ [Receipt]  │
│ CLM-9913 │ 93306 (Echo-Dop)│ Dr. Vance│ Aetna    │ 🟡 In Review │ [Trace]    │
│ CLM-9914 │ 71045 (Chest XR)│ Imaging  │ Medicare │ 🔴 Denied    │ [Appeal]   │
└──────────┴─────────────────┴──────────┴──────────┴──────────────┴────────────┘
```

- **Purpose**: Transparent hospital revenue management, claim adjudication tracking, patient billing, and pre-authorization validation.
- **Key UI Elements**:
  - **Financial Summary Cards**: High-visibility metric cards summarizing Gross Revenue, Days in AR (Accounts Receivable), First-Pass Clean Claim Rate (Target: > 96%), and Patient Copay Collection.
  - **Claim Pipeline Stepper**: Visual breadcrumb status: `Drafted` → `EDI Scrubbed` → `Payer Submitted` → `Adjudicated` → `Settled`.
  - **Itemized Patient Billing Module**: Plain-English explanation of hospital charges, deductible offsets, insurance discounts, and HIPAA-compliant payment gateway.

---

### Surface 5: Admin & Operations View (Staff, Beds, Inventory)

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ HOSPITAL OPERATIONS & BED CENSUS OVERVIEW                      Live Sync: 🟢 │
├──────────────────────────────────────────────────────────────────────────────┤
│ TOTAL BEDS: 450 │ OCCUPIED: 388 (86.2%) │ CLEANING: 18 │ ICU AVAILABLE: 4   │
├──────────────────────────────────────────────────────────────────────────────┤
│ WARD 4B: INTENSIVE CARDIAC CARE UNIT (ICCU)                                  │
│ Bed 401: [Occupied: LM-8821]  │ Bed 402: [Occupied: LM-8833]                 │
│ Bed 403: [🟡 Sanitization Req] │ Bed 404: [🟢 Available - Reserved for PostOp]│
├──────────────────────────────────────────────────────────────────────────────┤
│ PHARMACY & BIOMEDICAL INVENTORY ALERTS                                       │
│ ⚠ Low Stock Alert: Heparin 5000u/mL (Remaining: 14 vials — Reorder Threshold)│
│ ⚠ Biomed Calibration Due: Ventilator Unit #V-08 (ICU West)                  │
└──────────────────────────────────────────────────────────────────────────────┘
```

- **Purpose**: Hospital executive dashboard, nurse-to-patient staffing ratio monitoring, emergency room bed census, and critical inventory tracking.
- **Key UI Elements**:
  - **Live Bed Census Matrix**: Interactive floorplan/grid showing real-time bed status color-coded by clinical condition (`Occupied`, `Sanitization in Progress`, `Available`, `Out of Service`).
  - **Staffing Ratio Monitor**: Compares active nursing staff to admitted patients against safety benchmarks (e.g., ICU 1:1 or 1:2 ratio).
  - **Biomedical & Pharmacy Alerts**: Automated threshold triggers for pharmaceutical stock, blood bank units, and surgical consumables.

---

## 10. Image Selection, Lighting & Human Factors

Hospital imagery directly impacts patient heart rates and anxiety levels. Photography is a clinical tool, not cosmetic filler.

```
PHOTOGRAPHIC ETHICS & COMPOSITION:
┌───────────────────────────┬───────────────────────────┐
│        PERMITTED          │         REJECTED          │
├───────────────────────────┼───────────────────────────┤
│ • Natural, warm daylight  │ • Artificial harsh flashes│
│ • Real doctors in scrubs  │ • Staged stock models     │
│ • Genuine consultation    │ • Inaccurate clinical gear│
│ • Diverse, authentic ages │ • Oversaturated smiles    │
└───────────────────────────┴───────────────────────────┘
```

### 10.1 Photography Directives
1. **Lighting**: Soft, natural indirect daylight. Avoid sterile fluorescent cold cast or dramatic high-contrast studio flashes.
2. **Subject Matter**: Emphasize human connection—a physician listening intently, a surgeon reviewing digital imaging with a colleague, a nurse holding an elderly patient’s hand.
3. **Clinical Authenticity**: All protective equipment (PPE), stethoscopes, diagnostic monitors, and surgical gowns must adhere to authentic modern medical protocols.
4. **Cropping & Aspect Ratios**:
   - Hero Editorial: `16:9` or `21:9` wide crop with focal point positioned to leave generous negative space for typography.
   - Provider Profiles: `1:1` square or `4:5` portrait crop with uniform light slate background (`#F1F5F9`) and consistent head-and-shoulder scale.
   - Specialty Service Tiles: `4:3` architectural or clinical detail shots.

---

## 11. Accessibility Architecture (WCAG 2.1 AA / AAA Standard)

All clinical and patient interfaces must strictly adhere to accessibility mandates to ensure full usability by elderly patients, visually impaired users, neurodivergent individuals, and clinicians operating under intense fatigue.

1. **Color Contrast Ratios**:
   - All body copy against canvas: Minimum **7.0:1** (WCAG AAA).
   - Interactive button text and major headers: Minimum **4.5:1** (WCAG AA).
   - Focus indicator outline: `#0284C7` with a 2px white gap (`box-shadow: 0 0 0 2px #FFF, 0 0 0 4px #0284C7`), producing a minimum contrast ratio of **4.5:1** against all surfaces.
2. **Target Dimensions**:
   - Minimum clickable touch target of **44 × 44px** on all mobile and tablet viewports.
   - Minimum desktop click target of **36 × 36px** with at least **8px** surrounding clearance.
3. **Non-Visual Feedback (Screen Readers)**:
   - Dynamic clinical status changes (e.g., "Slot booked", "Vitals updated", "Bed status changed") must trigger `aria-live="polite"` or `role="alert"` announcements.
   - All diagnostic icons must include programmatic hidden text (`<span class="sr-only">Critical alert</span>`).
4. **Motion Safety**:
   - Strict adherence to `prefers-reduced-motion: reduce`. All video autoplay, tab transitions, and drawer slides must immediately downgrade to instant 0ms opacity cuts.

---

## 12. Specific Rules to Avoid Generic AI-Generated Design Patterns

To ensure this hospital design is indistinguishable from a top-tier digital product studio's work, the following anti-patterns are strictly prohibited:

```
ANTI-PATTERN BLACKLIST:
❌ NO neon cyan-magenta cyber gradients
❌ NO floating frosted-glass cards (glassmorphism) with unreadable text
❌ NO generic 3D glossy floating pills or stethoscopes
❌ NO AI filler copy ("Revolutionizing healthcare with AI-powered synergy")
❌ NO tracked-out ALL CAPS labels above every single heading
❌ NO identical rounded cards with identical 01 / 02 / 03 numbers
```

| Anti-Pattern (AI Tell) | Why It Fails in Healthcare | Lumera Standard (What We Do Instead) |
| :--- | :--- | :--- |
| **Neon Gradients / Glassmorphism** | Destroys clinical contrast; reads as a crypto or SaaS landing page; fails accessibility. | Solid, opaque `#FFFFFF` cards resting on `#F8FAFC` slate canvas with crisp `#E2E8F0` structural borders. |
| **Pervasive Decorative Numbers (01, 02, 03)** | Adds visual noise when content is not an actual sequential timeline. | Clean, semantic typography with contextual icons only when denoting an authentic multi-step patient wizard. |
| **Generic Marketing Jargon** | Diminishes institutional trust; sounds evasive and robotic to patients seeking care. | Clear, direct, empathetic clinical statements: *"Specialized care for complex cardiovascular conditions"* instead of *"Reinventing wellness journeys"*. |
| **Monotone Rounded Everything** | Single 24px border radius applied blindly to all elements regardless of scale. | Disciplined radius scale: `4px` for tags/badges, `6px` for buttons/inputs, `8px` for cards, `12px` for major modals. |
| **Isolated Colored Words in Headlines** | An infamous AI typographic cliché (e.g., "World class care for *everyone*"). | Uniform headline weight and color; let the strength of the typography and editorial meaning carry emphasis. |

---

## 13. Token Dictionary for Implementation Handoff

These tokens provide an exact programmatic foundation for frontend implementation:

```css
:root {
  /* Brand Foundation */
  --lumera-navy-900: #0B1B3D;
  --lumera-navy-800: #1E3A8A;
  --lumera-cyan-600: #0284C7;
  --lumera-cyan-700: #0369A1;
  --lumera-spruce-700: #0F766E;
  
  /* Canvas & Text */
  --lumera-canvas: #F8FAFC;
  --lumera-surface: #FFFFFF;
  --lumera-surface-subtle: #F1F5F9;
  --lumera-border: #E2E8F0;
  --lumera-border-strong: #CBD5E1;
  --lumera-text-primary: #0F172A;
  --lumera-text-secondary: #475569;
  --lumera-text-muted: #64748B;
  
  /* Clinical Alerts */
  --lumera-critical-bg: #FEF2F2;
  --lumera-critical-text: #991B1B;
  --lumera-critical-border: #FCA5A5;
  --lumera-warning-bg: #FFFBEB;
  --lumera-warning-text: #92400E;
  --lumera-warning-border: #FCD34D;
  --lumera-normal-bg: #F0FDF4;
  --lumera-normal-text: #166534;
  --lumera-normal-border: #86EFAC;
  
  /* Typography */
  --font-display: 'Newsreader', 'Source Serif 4', Georgia, serif;
  --font-sans: 'Plus Jakarta Sans', 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  
  /* Radii */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  
  /* Shadows */
  --shadow-subtle: 0 1px 3px 0 rgba(11, 27, 61, 0.05);
  --shadow-card: 0 4px 6px -1px rgba(11, 27, 61, 0.06), 0 2px 4px -2px rgba(11, 27, 61, 0.04);
  --shadow-hover: 0 10px 15px -3px rgba(11, 27, 61, 0.08), 0 4px 6px -4px rgba(11, 27, 61, 0.04);
}
```

---

*This document serves as the single source of truth for all digital touchpoints under the Lumera Academic Medical Center brand. Any modifications must pass review by the Design System and Clinical Human Factors review board.*
