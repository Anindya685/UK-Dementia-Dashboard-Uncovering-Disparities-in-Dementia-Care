# UK Dementia Dashboard: Illuminating Dementia Care Patterns for Public Understanding

## Overview
This project presents a comprehensive Tableau dashboard designed for public dissemination, particularly for an international news agency website. It offers a detailed, yet accessible, overview of dementia care in the UK. The dashboard aims to provide a high-level, insightful narrative of dementia prevalence patterns, diagnostic rates, demographic distributions, and prescribing practices. Its static, yet rich, visual design allows for immediate comprehension of key data points, making complex healthcare information digestible for a broad audience.

## Why This Project is Relevant
For the general public, and especially for news agency audiences, understanding the nuances of dementia care is crucial for informed citizenship, personal health decisions, and advocating for better services. This dashboard is highly relevant because it:

Facilitates Public Awareness: Provides a clear and immediate understanding of critical dementia care metrics, helping to raise public awareness about the disease's impact across the UK.

Informs Personal & Family Decisions: Highlights demographic trends and risk factors, such as the disproportionate burden on elderly women, which can inform families and individuals.

Supports Advocacy: Offers data-driven insights into diagnostic inequalities (e.g., ethnic disparities) and prescribing variations, providing evidence for advocacy groups pushing for equitable and safer care.

Enhances Accountability: By presenting official statistics in an accessible format, it enables citizens to understand and potentially benchmark their local areas, fostering a sense of public accountability for healthcare performance.

Streamlines Communication: Presents complex healthcare data in an intuitive and narrative-driven format, making it easier for news agencies to communicate crucial insights to diverse global audiences.

## Research Objectives
This dashboard was developed to achieve the following key objectives for public audiences and news agencies:

To provide an executive-level overview of dementia diagnosis rates and prevalence patterns across UK regions.

To highlight key demographic distributions (age, gender, ethnicity) of dementia diagnoses, exposing potential inequalities.

To illustrate clinical patterns such as the distribution of dementia subtypes.

To reveal regional variations in antipsychotic prescribing practices, raising awareness about medication management.

To offer a clear, data-driven narrative on the state of dementia care, simplifying complex healthcare information for immediate comprehension.

## Methodology
This project leverages Tableau's visualization capabilities to present a clear and concise "dashboard" of dementia care activity. The methodology focuses on immediate data comprehension and a structured visual flow to guide users through key insights with minimal interaction, adhering to newsroom communication standards.

## Data Sources and Features
Datasets were taken from: Primary Care Dementia Data September 2024 (https://digital.nhs.uk/data-and-information/publications/statistical/primary-care-dementia-data/september-2024). This dataset carries NHS England's Official Statistics designation, ensuring robust completeness and reliability.

Prevalence Data: Comprehensive coverage of dementia prevalence patterns.

Diagnostic Rates: Data on diagnosis rates for over-65 populations, including national benchmarks and regional variations.

Demographic Distributions: Detailed information on patient age, gender, and ethnic representation.

Prescribing Practices: Data on antipsychotic prescribing for both diagnosed and undiagnosed patients.

Clinical Data: Categorization of dementia subtypes.

## Key features derived from such data include:
Geographic distribution of diagnosis rates: Highlighting regional disparities across integrated care boards.

Dementia cases by age and gender: Illustrating exponential increases in late-life diagnoses and female predominance.

Ethnic distribution of diagnoses: Exposing potential under-representation in recorded diagnoses for minority communities.

Breakdown of dementia subtypes: Confirming proportions that mirror established clinical literature.

Regional antipsychotic prescribing variations: Comparing usage rates between diagnosed and undiagnosed patients.

## Data Pre-processing
Standard data pre-processing steps were crucial for ensuring data quality and usability, particularly for a public-facing dashboard:

Data Extraction: Collecting relevant data directly from the NHS Digital publication.

Data Cleaning: Employing Excel 365 with Power Query to execute systematic transformations, including:

Systematic removal of banner rows and asterisk suppression markers.

Conversion of percentage strings (e.g., "64.8%") to decimal format.

Standardization of all geographic identifiers as ons_code.

Data Anonymization/Pseudonymization: Ensured by NHS England's Official Statistics designation, satisfying patient privacy and compliance requirements.

Data Transformation: Aggregating practice-level data for antipsychotic prescribing and care planning to integrated care board level for analytical consistency. A synthetic snapshot_year field (set to 2024) enabled cross-table joins.

Categorization: Performing left joins on ons_code and snapshot_year to combine six cleaned tables into a single consolidated dataset. Null values (comprising less than 3%) were flagged rather than eliminated to preserve analytical transparency.

Output: The resulting seven-tab workbook was published directly to Tableau Public as the dashboard's sole data source.

## Data Processing/Analysis/Methods Used
The primary methods employed are Data Visualization and Interactive Storytelling within Tableau, with a strong emphasis on immediate comprehension and minimal user interaction for a public audience.

Geographical Mapping: A blue-gradient choropleth map encodes diagnosis rates, enabling instant recognition of geographic disparities (darker shading for higher coverage).

Key Performance Indicators (KPIs): Integrated into the narrative, such as the national 65% diagnosis rate benchmark.

Bar Charts:

A grouped bar chart ("Dementia Cases by Age and Gender") illustrates exponential increases in late-life diagnoses and female predominance.

A horizontal bar chart ranks dementia subtypes for easy comparison without requiring numerical literacy.

Pie Chart: Used to display ethnic distribution, appropriate for four distinct major categories, to highlight diagnostic inequalities.

Slope-Line Visualization: Captures regional antipsychotic prescribing variations, comparing usage rates between diagnosed and undiagnosed patients with colored markers, accentuating disparities through pre-attentive pattern recognition.

Visual Design Principles:

Newsroom Communication Standards: Titles follow sentence structure mimicking BBC editorial style (e.g., "Dementia Diagnosis Rates by Region (2024)").

Brand Palettes: The NHS blue-green palette reinforces institutional trust.

Limited Interactivity: User interaction is limited to hover tooltips, maintaining a low cognitive load for general audiences.

## Technologies Used
Tableau Public: The platform used for developing and sharing the interactive dashboard, chosen for its accessibility and strong visualization capabilities.

Microsoft Excel (with Power Query): Used for robust data preparation, cleaning, transformation, and initial aggregation prior to connection with Tableau.

## Key Findings
While specific findings are best appreciated through interaction with the live dashboard, this project prominently highlights:

Significant Geographic Disparities in Diagnosis Rates: London and South East regions consistently exceed the national 65% benchmark, while rural areas in the North-East and South-West lag behind, indicating systemic under-recognition.

Exponential Rise in Diagnoses with Age and Female Predominance: Diagnoses dramatically increase after age 75, with women consistently comprising two-thirds of diagnoses in the oldest age cohorts.

Stark Ethnic Diagnostic Inequalities: Black, South Asian, and Mixed heritage communities show significant under-representation in recorded diagnoses despite evidence of equal or higher disease risk, indicating a systematic diagnostic gap.

Consistent Clinical Subtype Proportions: Alzheimer's disease dominates (approx. 42%), followed by vascular (15%) and Lewy body (3%) dementias, confirming data authenticity.

Twofold Regional Variation in Antipsychotic Prescribing: North-West England shows peak prescribing rates, reinforcing concerns about unsafe prescribing practices and regional healthcare inequities.

## Recommendations
Based on the compelling insights the dashboard provides, potential recommendations for public awareness, policy, and advocacy could include:

Targeted Public Health Campaigns: Launching campaigns focused on rural areas and minority communities to improve awareness and reduce diagnostic barriers.

Culturally Sensitive Memory Services: Developing and promoting services that are accessible and culturally appropriate for Black, South Asian, and Mixed heritage communities to address diagnostic inequalities.

Enhanced Support for Elderly Women: Focusing resources on support and early intervention programs for older women, given their disproportionate burden of disease.

Review of Prescribing Practices: Investigating and addressing regional variations in antipsychotic prescribing to ensure safe and appropriate medication management.

Empowering Citizens: Providing accessible data enables citizens to benchmark their local areas and demand accountability from healthcare providers, fostering informed advocacy.


## How to View the Dashboard
The interactive dashboard is publicly available on Tableau Public.
You can access and interact with the dashboard here:

🌐 UK Dementia Dashboard: Dementia UK Insights on Tableau Public (https://public.tableau.com/app/profile/anindya.swain4442/viz/UKDementiaDashboardInternationalNewsAgency/DementiaUKInsights)
