# MS Data Journalism Thesis: “Why It’s So Hard To Know How Often AI Goes Wrong – And What That Means For Accountability When Algorithms Harm People” – Data Analysis Repo

## Project Overview
This repository contains the code, data, and supporting materials for my MS Data Journalism (Columbia University, Class of 2025) thesis  “Why It’s So Hard To Know How Often AI Goes Wrong – And What That Means For Accountability When Algorithms Harm People.” The project centers on systematic analysis of the Artificial Intelligence Incident Database (AIID), one of the world’s largest publicly available datasets of real-world problems and harms caused by AI systems. This analysis aims to surface patterns, gaps, and challenges in recording and understanding AI-related incidents—informing both academic research and policy discussions around AI accountability.

## Motivation
AI systems are increasingly embedded in high-stakes decisions across domains like law enforcement, healthcare, welfare, and finance. Failures or unintended outcomes can have substantial impact on individuals and communities, yet information about such incidents is often scattered, underreported, or hidden. The thesis explores:

- Why most failures of AI harm are not systematically counted or tracked

- How “incident databases” like the AIID can help (and what their limits are)

- Patterns of AI incidents by geography and sector

- Barriers to effective transparency and accountability for algorithmic harm

## Data Sources
[AI Incident Database (AIID)]([url](https://incidentdatabase.ai/))

Main source—downloaded full database snapshot (CSV files)

Includes detailed records of AI failures/incidents reported globally, spanning various sectors and years

MIT AI Risk Repository: Cross-referenced to supplement classification schemes

Other references: OECD frameworks, journalistic and academic commentaries for context and framing

## What You’ll Find Here
analysis.ipynb: Main Jupyter notebook containing all data handling, cleaning, exploratory analysis, and visualizations.

Reads all key CSVs, processes dates/locations/sectors

Produces breakdowns and plots by year, country, US state, sector, and key metadata fields

Data pre-processing scripts: Cleaning location fields, standardizing country/state codes, reconciling missing data.

Outputs: Visualizations (e.g., incidents over time, top countries, sectors), exportable tables for use in GIS or reporting tools.

## Key Steps in the Analysis
- Loading and Cleaning Data:
The AIID and its associated classification tables are imported. Code adapts for known issues: inconsistent date/location formats, missing country codes, diverse reporting styles.

- Temporal Analysis:
Plots annual and monthly incident counts to identify when AI incidents have been reported most frequently. Includes cautions about future-dated/testing entries.

- Geographical Analysis:
Extracts, standardizes, and visualizes incident locations—first by country, then (for US) by state, and adapted for global mapping. Highlights strong reporting bias toward richer, Western countries with active AI journalism/advocacy presence; many entries are “Global” or lack location data.

- Sectoral Analysis:
Breaks down incidents by industry sector. Patterns reveal overrepresentation in fields like “information and communication,” “government,” and “transportation,” but far sparser reporting in finance, retail, education, hospitality, or healthcare—despite likely real-world harms being present.

- Critical Reflection:
The notebook and thesis chapter discuss why available data is only a partial portrait:

Crowdsourced and media-based reporting—biases toward tech-savvy and resource-rich regions/sectors

Often no mandatory incident reporting outside select high-risk domains

Most harmful outcomes go unreported, uninvestigated, or are invisible to both public and regulators

## Usage
Run analysis.ipynb in a Jupyter environment with the full data directory as specified, making sure all CSVs are extracted and available.

Outputs include plots for thesis visualization, CSVs for QGIS mapping, and tabular breakdowns.

All analysis code is fully transparent and can be modified for further research or adapted to additional incident datasets.

## Limitations and Ethics
Coverage Bias: The AIID is not a census, but an archive of “incidents logged, not incidents occurred.” Statistical findings reflect patterns of visibility, not true incident frequency.

Incomplete Records: Many records lack geographic or sectoral metadata entirely, especially for non-Western countries and non-government/IT industries.

Responsible Use: This analysis cannot be used to make definitive claims about country-level prevalence or relative sectoral risk. Rather, it is a diagnostic tool for highlighting gaps, directions for further investigation, and the urgent need for systematic incident reporting in AI deployment.

Privacy: Individual cases are anonymized in line with the AIID policies. Where real-world stories are mentioned, they are used with attribution to public reporting and documented sources.

## References
[AI Incident Database (AIID)]([url](https://incidentdatabase.ai/))

Further background, methodology, interviews, and discussion are detailed in the full thesis writeup.

## Citation
If using this code or data approach for academic, journalistic, or policy research, please cite the thesis and the AI Incident Database as credited in your publication guidelines.
