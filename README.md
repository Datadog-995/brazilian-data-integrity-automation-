 Brazilian E-Commerce Data Integrity & Automation Pipeline

## 📌 Project Overview
This project establishes an automated data integrity and data scrubbing pipeline for a complex, multi-table Brazilian e-commerce dataset. Instead of relying on manual data cleaning, this repository demonstrates a scalable, programmatic workflow designed to ingest raw data, enforce strict integrity constraints, track transformations, and output analysis-ready datasets.

### Data Pipeline Scale: Records Processed by Table
<img width="1600" height="889" alt="Brazilian_ECommerce_Scale" src="https://github.com/user-attachments/assets/b1f0b644-d056-4026-bb0e-4d169bf72808" />
*Figure 1: Visual mapping of data ingestion scale across all nine Olist relational database tables.*
## 🛠️ The Toolset & Workflow
*Figure 2: Distribution of transaction modalities, highlighting credit card dominance.*

<img width="1000" height="700" alt="payment_methods_pie_chart" src="https://github.com/user-attachments/assets/064885f5-34ad-4e80-9823-13c2d529feb2" />

The pipeline utilizes a coordinated, multi-tool architecture to maximize efficiency and handling capacity:
*   **OpenRefine:** Used for initial schema evaluation, text standardizations, and complex text clustering/faceting.
*Figure 3: Breakdown of leading commercial product categories, validating programmatic text standardization.*

<img width="1000" height="700" alt="top_products_pie_chart" src="https://github.com/user-attachments/assets/a2391098-067e-4b44-9a0a-1762d74923a9" />

*   **Google Colab & Python (Pandas):** The core engine executing programmatic, reproducible scripts to handle automated missing-value imputation, data type enforcement, and duplicate detection.
*   **Google Sheets:** Leveraged for final reporting, presentation-layer formatting, and AI-assisted change logs.

## 🗂️ Data Architecture & Integrity Challenges
The raw Brazilian dataset presented several distinct data integrity hurdles that this pipeline automatically resolves:
*   **Localization & Encoding:** Standardizing Portuguese text strings, accents, and special characters across millions of rows.
*   **Schema Standardization:** Aligning data types, handling regional zip code formats, and verifying localized currency fields.
*   **Relational Consistency:** Ensuring referential integrity across related tables (e.g., matching customer IDs, order IDs, and seller IDs seamlessly without data loss).

## 🚀 How the Pipeline Works
1. **Ingestion & Profiling:** Raw CSV/JSON files are profiled to detect anomalies, data drift, and structurally corrupted records.
2. **Automated Scrubbing:** Python scripts programmatically drop unrecoverable duplicates and fill missing values using logical business rules.
3. **Validation Check:** A final programmatic audit ensures all text is scrubbed, data types match target schemas, and primary/foreign keys align perfectly.

## 📈 Portfolio Business Impact
By shifting from manual data cleaning to an **automated data integrity solution**, this workflow reduces data preparation time by an estimated 70-80%, guaranteeing that downstream analytics or machine learning models operate on 100% reliable data.

