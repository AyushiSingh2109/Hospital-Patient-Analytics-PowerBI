# Hospital Patient Analysis — Power BI Project

## Project structure
```text
PowerBI-Hospital-Patient-Analysis/
├── README.md
├── Dataset/
│   └── patient_data_template.xlsx
├── PowerBI/
│   └── Hospital_Patient_Analysis.pbix
├── Screenshots/
│   ├── README.md
│   └── background_*.png
└── Report/
    └── Project_Report.pdf
```

## Project overview
This project analyzes hospital patient, admission, clinical outcome, and financial information using Microsoft Power BI.

The uploaded PBIX was inspected. It contains four report pages:
- Hospital Executive Overview & Patient Analytics
- Clinical Operations & Financial Breakdown
- Patient Outcomes & Discharge Analytics
- Page 1

The report visuals reference a `Patient_Data` table and fields including patient ID, admission date/type, department, doctor, city, gender, age group, diagnosis, ward type, insurance type, outcome, length of stay, room charges, medication cost, lab-test cost, treatment cost, and total cost.

## Objectives
- Monitor patient volume and admission patterns.
- Compare patient counts across departments, cities, diagnoses, and admission types.
- Review length of stay and patient outcomes.
- Analyze hospital revenue and cost components.
- Compare performance across wards, doctors, and insurance categories.

## Data and limitations
`Dataset/patient_data_template.xlsx` is a **column template**, not the original dataset. The uploaded PBIX contains an embedded Power BI data model, but the underlying source rows could not be exported directly in this environment. No patient records or KPI values have been fabricated. If your instructor requires the raw dataset, open the PBIX in Power BI Desktop and export the `Patient_Data` table to this workbook.

## Data cleaning
The exact Power Query transformation steps are not exposed in the report definition inspected here. Document only the steps you actually performed in Power Query (for example: data type correction, duplicate handling, missing-value treatment, date formatting, and category standardization). Do not claim a cleaning operation unless it was performed.

## Data model
The report visuals use a table named `Patient_Data`. The relationships and full model diagram should be verified in Power BI Desktop's Model view before submission.

## DAX measures
The report references the following measures. Their exact DAX definitions should be copied from the PBIX Model view (right-click each measure → copy formula) before claiming these are the original formulas:
- Total Patients
- Total Revenue
- Average Bill per Patient
- Average Length of Stay
- Total Room Charges
- Total Medication & Lab Cost
- Total Treatment Cost
- Long Stay Patient Count
- Recovery Rate %
- Avg Daily Patient Cost
- Total Admissions
- Highest Admission Month
- Lowest Admission Month
- Top Department / Diagnosis / City / Insurance / Doctor
- Lowest Department / Diagnosis

## Screenshots
The Screenshots folder includes background images embedded in the PBIX, not screenshots of rendered report pages. To create authentic screenshots:
1. Open `PowerBI/Hospital_Patient_Analysis.pbix` in Power BI Desktop.
2. Select each report page.
3. Use **File → Export → Export to PDF**, or take a screenshot with Snipping Tool.
4. Save the relevant page captures in this folder (for example `dashboard.png`, `clinical_financial.png`, and `patient_outcomes.png`).

## How to open
1. Install Microsoft Power BI Desktop.
2. Open `PowerBI/Hospital_Patient_Analysis.pbix`.
3. Wait for the model to load. If prompted for a data source, follow the original source connection details.
4. Review the report pages and refresh only if the original data source is available.

## Submission checklist
- [ ] Enter student name and registration number in the PDF.
- [ ] Export the actual patient dataset if required.
- [ ] Verify model relationships and copy exact DAX formulas from Power BI.
- [ ] Add genuine report-page screenshots.
- [ ] Confirm the PBIX opens correctly on the submission computer.
