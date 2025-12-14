# Grant Funding Analysis for Community Charities

## Project Context

A small community charity in Cornwall supporting low-income families needs to identify realistic funding opportunities for organizational development.

## Business Problem

**Challenge:** With limited resources and no dedicated fundraising staff, the charity must strategically focus on grant applications most likely to succeed.

**Questions:**
1. **Which focus areas attract most grant funding?**  
   Should we emphasize poverty relief, community support, education, or another cause?

2. **What grant amounts are realistic for community charities?**  
   What funding levels should we target to maximize chances of success?

3. **Who funds community charities: government or private funders?**  
   Where should we direct our application efforts?

## Geographic Context

**Location:** Cornwall, South West England  
**Characteristics:** Rural area, lower average income, limited local funding sources

## Data Source

**Dataset:** [360Giving GrantNav](https://grantnav.threesixtygiving.org/)  
**Period:** 2022-2025 
**Scope:** UK charitable grant awards

**Note:** Raw data file not included in repository due to size. Download from 360Giving and place in `data/` folder.

## Methodology

**Analysis Focus:**
- Charity and nonprofit recipients only (excluding individual grants)
- Community-scale grants (£1,000 - £100,000 range)
- Comparable organizations (small-medium charities)

**Approach:**
- Descriptive statistics of grant distribution
- Segmentation by cause area and funder type
- Geographic analysis (South West region focus)

## Project Structure
```
Charity_Grant_Analysis/
├── data/
│   └── 360giving_grants.csv (not included)
├── notebooks/
│   └── 01_data_exploration.ipynb
├── outputs/
├── README.md
└── .gitignore
```

## Key Research Questions

### 1. Focus Area Identification
Analyze grant distribution across different cause categories to identify areas with strongest funding support.

### 2. Realistic Grant Sizing
Determine typical grant amounts for community charities to set appropriate funding targets.

### 3. Funder Type Analysis
Compare government vs. charitable trust funding to optimize application strategy.

## Expected Outcomes

**Practical Recommendations:**
- Suggested focus area(s) for charity development
- Target grant range for applications
- Priority list of potential funders
- Geographic considerations for Cornwall-based charity

## Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **matplotlib** - Data visualization
- **Jupyter Notebook** - Interactive analysis environment

## Project Status

🚧 **In Progress** - Initial data exploration phase

## Author

Data Analyst Apprentice (Corndel Level 4)  
📍 Falmouth, UK

## License

Educational project. Data source: 360Giving (Open Data).

---

*This analysis aims to provide evidence-based guidance for small charities navigating the UK grant funding landscape.*
```
