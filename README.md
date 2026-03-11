Bus Fare Cap Policy and School Attendance
This project investigates whether the UK government's 2023–24 bus fare cap — which limited single bus fares to £2 — had a measurable effect on school attendance in areas with high bus usage.
Background
The bus fare cap was introduced in January 2023 and extended through 2024 before being partially wound down in 2025. The policy was designed to improve public transport affordability, particularly for lower-income households. Given that many secondary school pupils rely on bus travel, the hypothesis was that reduced fares might improve attendance by lowering a practical barrier to getting to school.
Data
The analysis draws on three publicly available administrative datasets:

DfE school attendance data (termly, local authority level) — overall absence, unauthorised absence, and persistent absence rates, disaggregated by school type and Free School Meals (FSM) eligibility
DfT bus usage data (annual, local authority level) — used as a proxy for exposure to the fare cap policy
Census 2021 car ownership data — used as a control variable reflecting local transport dependency

Rural/urban classification and a manual local authority to combined authority mapping were also used to harmonise geographies across datasets.
Methods
The original analytical design used a difference-in-differences (DiD) approach, treating London as a control group on the basis that the fare cap policy was less likely to affect behaviour in an area already covered by TfL fare structures. This approach was abandoned after the London data showed insufficient variance to serve as a viable control, producing near-zero regression coefficients.
The analysis was revised to use a paired samples t-test design, comparing attendance in approximately 60 Home Counties local authorities before and after the cap was introduced (Test 1) and before and after its removal (Test 2).
Findings
Results were inconclusive. Test 1 produced a statistically significant result with a small effect size, but Test 2 showed attendance continuing to rise after the cap was removed — casting doubt on whether the Test 1 result reflected a genuine policy effect. The most likely explanation is that the post-Covid attendance recovery trend acted as a confound: attendance was improving across the board during this period for reasons unrelated to the fare cap, and the two trends could not be disentangled with the available data.
A secondary finding — that FSM-eligible pupils in London had consistently higher absence rates than non-FSM pupils across all terms and school types — was statistically significant and practically meaningful, though this was not the primary research question.
Visualisations
The repository includes interactive HTML visualisations built with Bokeh:

A choropleth map of average absence rates across London boroughs
A trend line chart showing absence rates over time by FSM status, with a school type filter
An interactive bar chart of borough-level absence, filterable by period, school type, and FSM status

Limitations
The analysis is observational and cannot establish causation. The timing mismatch between termly attendance data and annual bus usage data is a significant constraint. Missing data for approximately one third of local authorities was not random, which limits generalisability. The study covers Home Counties local authorities only, reflecting local knowledge that the policy was more consistently enforced in those areas.

Data Sources/Links (correct as of February 2026)

School Attendance
Autumn 2022-23
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/4caacb6e-434c-4f49-bb15-5e7e02cc20bb
Spring 2022-2023
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/89db45b0-aa87-475c-aee1-1ea22cf6db14
Summer 2022-2023
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/ed0a4df7-4310-4e81-8fdc-05bce2ef6ad9
autumn 2023-2024
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/3273d4ff-1ea1-4ee6-b935-c89079fbfb01
spring 2023-2024
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/62f500ba-a6f9-4570-8283-3d4465e45923
summer 2023-2024
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/8ba277ea-0dae-4544-9c29-08e8320bce97
autumn 2024-2025
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/5deec375-12e8-48d9-95ae-b6e52e486ec2
spring 2024-2025
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/4463ab3e-d45e-48a7-be7a-1d6d4a1daa11
summer 2024-2025
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/f18b1a03-0c47-4f1c-bcb6-ba58f31aca37

other datasets

Car usage
https://www.ons.gov.uk/datasets/TS045/editions/2021/versions/4
Bus usage
https://www.gov.uk/government/statistical-data-sets/bus-statistics-data-tables?utm_source=chatgpt.com
urban/rural
https://www.data.gov.uk/dataset/bb9553f2-74a6-46b8-b77c-0ec6b61acd1e/rural-urban-classification-2021-of-local-authority-districts-2021-in-ew?utm_source=chatgpt.com
IMD
https://www.gov.uk/government/statistics/english-indices-of-deprivation-2025
LA codes
https://www.data.gov.uk/dataset/2ea56d0b-131a-484c-b1c8-36f41189cc5a/local-authority-districts-december-2021-boundaries-ew-buc-and-rural-urban-classification
