# Project 01 Data Analysis Refresh

Objective
Exploratory data analysis to extract insights from a real dataset.

Tools
- Python (pandas, matplotlib)
- SQL
- Excel / Data Visualization
- PowerBi Desktop
- Csv (for Market.csv use this link https://drive.google.com/file/d/10JkVvc6zaK9YbuRC5NrPRZqXUCl6MQQx/view?usp=sharing)

Description
This project is part of my Data Analyst skill refresh after completing a professional bootcamp.
The goal is to rebuild fluency with real data and focus on clarity rather than perfection.

Status
Work in progress – insights and structure will be improved iteratively.


## Refresh Notes – Data Model Review

### Market table
- Identified 3 columns likely unused for analysis
- Need to confirm whether they are required for any visuals or measures

### Country table
- Two columns represent the same concept (absolute value vs percentage)
- Potential redundancy – normalization or single source of truth needed

### Data Model
- Primary key structure not clearly documented
- Need to review which columns uniquely identify records
- Relationships currently working but require validation

### Next steps
- Validate primary keys
- Simplify tables where possible
- Review visual interactions after data model cleanup


## Refresh Notes - Day 2
### Overview Page Interactions
- Enabled cross-filtering between all main visuals
- Verified that selecting a market updates other charts correctly
- Noted that some slicer interactions depend on data model relationships

### Inflation Analysis Pages
- Confirmed table-to-visual filtering works correctly
- Observed that selecting dates not present in other visuals leads to no change (expected behavior)

### Predictive Analysis Page
- Reviewed map interactions and zoom behavior
- Fixed zoom issue on inflation prediction map
- Noted minor color/interaction inconsistencies for future refinement
