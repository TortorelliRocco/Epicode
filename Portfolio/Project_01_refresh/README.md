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


## Predictive Analysis – Interaction Refinement - Day 3
- Removed interactions between predictive chart and maps
- Prevented unintended color and filter conflicts
- Improved clarity and stability of predictive visuals


### Predictive Analysis Page
- Reviewed map interactions and zoom behavior
- Fixed zoom issue on inflation prediction map
- Noted minor color/interaction inconsistencies for future refinement


## Data Model – Market Table Analysis - Day 4
- Reviewed structure and purpose of the market table
- Identified the absence of a natural primary key; records are defined by a composite of country and time
- Clarified the role of ISO3, date fields, and geographic coordinates
- Confirmed market table acts as a fact table containing food price and inflation metrics
- Marked opportunities for future refactoring (date and geography dimensions)


## Data Model – Country and Details Tables Review - Day 5

### Country Table
- Contains time-based inflation data at country level
- Uses a composite key (ISO3 + Month + Year), resulting in a strong technical key but non-pure dimensional behavior
- Acts as a time-grained fact-like table rather than a pure country dimension
- Identified redundant inflation metrics (absolute vs percentage values)
- Includes date fields that overlap conceptually with market table

### Details Table
- Small summary table (one row per country)
- Provides aggregated country-level indicators used for comparative analysis
- Acts as a hub table connecting market and country tables
- Structure supports high-level insights despite limited row count

## Refresh Notes – Day 6 & Day 7 (Dashboard Refinement)

### Internationalization
- Translated the entire dashboard from Italian to English
- Standardized titles, labels, slicers, and visual text
- Improved international readability and portfolio suitability

### UX & Visual Improvements
- Added tooltips to navigation buttons on each page
- Removed data labels from overview visuals to reduce clutter
- Reviewed and fixed visual interactions across pages
- Disabled unintended interactions affecting predictive maps

### Date & Formatting Consistency
- Standardized date formats across all tables and visuals
- Replaced long textual date formats with numeric formats
- Ensured consistent behavior between tables, slicers, and charts

### Map Visuals
- Verified that market-level maps clearly display market names on hover
- Improved zoom and selection behavior in predictive and overview maps

Status update:
The dashboard is now fully translated, visually consistent, and structurally stable.
Ready for portfolio review and alignment with PL-300 best practices.

## Refresh Notes - Day 8 
- Added initial DAX measures (averages and time intelligence) to improve analytical flexibility and align the project with PL-300 best practices.
