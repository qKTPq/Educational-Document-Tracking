# Educational Document Tracking & Generation System

An automated, blueprint-driven framework designed to generate standardized, professionally formatted LaTeX assessment materials for long-term curriculum tracking. This system eliminates manual formatting overhead by linking document metadata directly to headers, tables, and version structures.

## 📌 System Architecture

The repository enforces a strict, scalable naming convention to allow precise tracking across multiple subjects and grade levels:

$$\texttt{[Student Code] - [Subject Code] - [Category Code] - [Chapter].[Item Sequence][Document Type]}$$

### Production-Ready Code Examples:
* **Primary 6 Science Midterm:** `YR-SCIP6-MT-1.01E`
* **Primary 6 Math Midterm:** `YR-MTHP6-MT-1.01E`

---

## 🛠️ Features

- **Automated Meta-Linking:** Change document parameters once in the configuration section; the system automatically updates the entire document header, context tracking table, and instruction banners.
- **Balanced Visual Hierarchy:** Optimized two-column `minipage` layouts that align student metadata tables with score summary blocks seamlessly.
- **Thai Language Ready:** Native rendering support for Thai script via XeLaTeX (`Laksaman` font integration) with clean line-breaking rules (`\XeTeXlinebreaklocale "th"`).
- **Zero-Dependency Fast Compilation:** High-speed rendering loops stripped of heavy barcode engines for streamlined local production.

---

## 📂 Subject & Document Directory Reference

### 1. Subject Codes
* `MTH` / `MTHP6` — Mathematics (General / Primary 6)
* `SCI` / `SCIP6` — Science (General / Primary 6)
* `PHY` / `CHM` / `BIO` — Physics / Chemistry / Biology
* `ENG` — English

### 2. Document Type Suffixes
* **Assignments:** `WS` (Worksheet) | `HW` (Homework) | `QZ` (Quiz) | `PQ` (Practice Questions)
* **Reference:** `LN` (Lecture Notes) | `CS` (Cheat Sheet) | `SG` (Study Guide)
* **Assessments:** `E` / `EX` (Exam) | `SM` (Summary) | `SN` (Solutions Key) | `RV` (Review Sheet)

---

## 🚀 Getting Started

1. Clone the repository.
2. Run the fast automation script:
   ```bash
   python generate_exam.py
