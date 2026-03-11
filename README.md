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
