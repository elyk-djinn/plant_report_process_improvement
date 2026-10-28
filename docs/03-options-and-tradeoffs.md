# 3. Options and trade-offs

## Option A: Managers encode straight into the raw data sheets

| Pros | Risks |
| --- | --- |
| Simple to set up, with no lookup formulas or extra tables | High risk of inconsistent entries, for example two spellings of the same scheme |
| Managers control how transactions are tagged | Hard to audit errors or trace them back |
| Flexible, since new schemes or card types can be added at once | Scalability problems as more people encode |
| Lowest upfront effort | More work for managers |

## Option B (the compromise I recommended)

Managers keep sending their pre-processed files. In addition, each sends a raw sheet taken directly from the system with the requested fields. The analyst pastes that raw sheet into the dashboard workbook.

Why this one: it asks little of the managers, the data comes from the system and not from retyping, and the inconsistency risk in Option A mostly disappears.

## What changes for each role

| Role | Before | After |
| --- | --- | --- |
| Managers | Send pre-processed data that gets processed again | Still send pre-processed data, plus a raw system sheet with the requested variables |
| Reports analysts | Update reports by hand from many file sources | Monitor data quality, verify raw sheets, troubleshoot formulas and links, manage dashboard logic |

## Time effect of Option B

Option B saves less than Option A, because some steps still involve a paste. It is the version that could actually be adopted.

| Process group | Legacy | Option B |
| --- | --- | --- |
| Purchase orders | 30 min | 2 min |
| Quality assurance data | 20 min | 1 min |
| Personalization received | 10 min | 2 min |
| Production data | 5 min | 2 min |

Reported total: 96 minutes down to 47 minutes of daily encoding work, about a 51% reduction.
