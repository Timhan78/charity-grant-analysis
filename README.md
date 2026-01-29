# Grant Funding Analysis for Community Charities

## Project Context
A small community charity in Cornwall supporting low-income families needs to identify realistic funding opportunities for organizational development.

## Business Problem
**Challenge:** With limited resources and no dedicated fundraising staff, the charity must strategically focus on grant applications most likely to succeed.

**Questions:**
1. Which focus areas attract most grant funding?
2. What grant amounts are realistic for community charities?
3. Who funds community charities: government or private funders?

## Key Findings

### Question 1: Realistic Grant Amounts
- **Typical grant: £10,000** (median £9,980, mode £10,000)
- 25% of grants: up to £4,361
- 75% of grants: up to £20,000
- **Recommendation:** Start with applications for £5,000-10,000

### Question 2: Top Focus Areas
Based on keyword classification of 112,516 grants:

- **Youth (children and young people):** 22,107 grants, £344M total
- **Health (mental health, wellbeing):** 17,253 grants, £258M total
- **Family:** 10,339 grants, £169M total
- **Elderly:** 10,529 grants, £159M total
- **Poverty:** 8,080 grants, £108M total
- **Refugee:** 2,684 grants, £49M total (highest average grant: £18,300)

**Recommendation:** Focus on Youth or Health for maximum opportunities

### Question 3: Government vs Private Funders
- **Private funders provide 89% of all funding and 93% of all grants**
- Grantmaking Organisations: £1,165M (63%)
- Lottery Distributors: £486M (26%)
- Central Government: £155M (8%) — fewer grants but higher average (£25,500)

**Top 5 funders by total amount:**
1. The National Lottery Community Fund — £386M
2. Garfield Weston Foundation — £125M
3. National Lottery Heritage Fund — £57M
4. Lloyds Bank Foundation — £45M
5. Sport England — £43M

**Recommendation:** Start with National Lottery Community Fund, then move to specialised funders

## Data and Methodology

### Data Source
- **Dataset:** 360Giving GrantNav
- **Period:** 2022-2024 (post-COVID)
- **Original size:** 449,414 grants

### Filtering Pipeline
| Stage | Dataset | Rows | What was removed |
|-------|---------|------|------------------|
| 0 | Raw data | 449,414 | — |
| 1 | Charity types only | 137,443 | Individuals, non-charity orgs |
| 2 | Grant size filter | 115,287 | Grants < £1K and > £100K |
| 3 | Final dataset | 112,516 | Universities, NHS, councils |

**Final dataset: 25% of original data**

### Classification Method
Used keyword matching to classify grants into 7 focus areas. Coverage: ~50% of dataset.

### Limitations
- Keyword classification covered only 50% of data
- No regional breakdown (Cornwall-specific analysis not included)
- Success rates not available in data
- Some grants may fall into multiple categories

## Project Structure
```
Charity_Grant_Analysis/
├── data/
│   └── 360giving_grants.csv (not included - download from 360Giving)
├── notebooks/
│   └── 01_data_exploration.ipynb
├── outputs/
├── README.md
└── .gitignore
```

## Technologies Used
- Python 3.x
- pandas — data manipulation and analysis
- seaborn, matplotlib — data visualisation
- Jupyter Notebook — interactive analysis

## Project Status
✅ **Completed** — Analysis finished, recommendations provided

## Author
Data Analyst Apprentice (Corndel Level 4)
📍 Falmouth, UK

## License
Educational project. Data source: 360Giving (Open Data).

---
*This analysis provides evidence-based guidance for small charities navigating the UK grant funding landscape.*