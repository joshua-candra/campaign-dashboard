# campaign-dashboard
The **Campaign Dashboard** is an interactive BI dashboard analyzing the evolution of American campaign finance from 1980 to 2024. This project transforms raw data into actionable insights regarding political ideology, PAC reliance, and Incumbent Advantage in federal and governor elections.

Data Source: **dime_recipients_1979_2024.csv.gz - Candidate/Recipient** scores at https://data.stanford.edu/dime.

### KPIs
There are six KPIs in this dashboard, including:
1. Total Raised: Total amount of money raised.
2. PAC Reliance %: The percent of donations from PACs (Political Action Committees).
3. Small-Dollar Reliance %: The percentage of donations that are unitemized (donations below $200).
4. Average Donation: Average amount of money donated per person.
5. Burn Rate: The financial health ratio between total spent and total raised (Total Disbursements / Total Receipts).
6. Average Ideology: The average ideological CFscore of all candidates.

### Charts
There are five charts in this dashboard, including:
1. Contribution Mix by Party (100% Stacked Bar Chart)
2. Incumbent vs Challenger Funding (Clustered Bar Chart)
3. Receipts by State (Filled Map)
4. Funds Raised Over Time (Ribbon Chart)
5. Ideology vs Fundraising (Scatter Plot)

### Data Source & ETL
This dashboard is powered by a custom PostgreSQL view generated via an automated ETL pipeline. The source code for the ETL pipeline can be found here: https://github.com/joshua-candra/campaign-etl-project.
