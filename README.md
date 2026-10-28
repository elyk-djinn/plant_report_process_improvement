# Standardizing a Daily Plant Report: 32 Manual Steps to 12

**Role:** Business Process Analysis Intern, CX Operations, Allcard Inc. (Jul to Sep 2025)
**Author:** Gene Kyle P. Solano
**Tools:** Excel (pivot tables, slicers, lookups, structured tables), Power BI (feasibility), process documentation

A daily plant report took 32 manual steps and 22 pages of instructions to produce. Every department sent data in a different format, so each day involved copying, pasting, reformatting and checking figures across many workbooks. I documented the process, designed a standard raw data format, and built an Excel dashboard that updates from linked raw data sheets.

## Results

| Measure | Before | After |
| --- | --- | --- |
| Process steps | 32 manual | 12 semi-automated |
| Daily encoding time (estimate) | 96 min | 47 min |
| Reduction in manual workload | | about 51% |
| Output | Static tables | Interactive dashboard with slicers |
| Error ownership | One person consolidates everything | Each department owns its own data sheet |

Time figures are estimates from the process-group timings in the proposal and cover the plant report only. The proposal was submitted on Aug 29, 2025. The decision on which version to adopt for daily use was still pending at that time.

## Where the time came back

| Process group | Legacy | Proposed |
| --- | --- | --- |
| Purchase orders | 30 min | 2 min |
| Quality assurance data | 20 min | 1 min |
| Personalization received | 10 min | 2 min |
| Production data | 5 min | 2 min |

These are the four largest reductions. Other groups, such as pending personalization and finalization, were left unchanged in this version.

## What I did

1. **Documented the as-is process.** Mapped the 32 steps into process groups and estimated daily minutes for each. See [docs/01-problem-and-legacy-process.md](docs/01-problem-and-legacy-process.md).
2. **Talked to the people doing the work.** The reporting team described repetitive encoding, mismatched formats, no raw data standard and static reports.
3. **Designed a standard raw data format.** One row per transaction, uniform headers, shared core fields. See [docs/02-standard-raw-data-format.md](docs/02-standard-raw-data-format.md) and the [CSV templates](templates/).
4. **Weighed two options.** Managers encoding directly was simple but risked inconsistent spellings and untraceable errors. The compromise keeps existing files and adds a raw system export per department. See [docs/03-options-and-tradeoffs.md](docs/03-options-and-tradeoffs.md).
5. **Built the dashboard in three iterations.** Charts, slicers, pivot tables and conditional formatting on top of dedicated raw data sheets. See [docs/04-dashboard-design.md](docs/04-dashboard-design.md).
6. **Tested the path to Power BI.** Looked at folder queries, slicers and refresh limits. See [docs/05-power-bi-feasibility.md](docs/05-power-bi-feasibility.md).
7. **Planned the rollout.** A decision for every sheet in the legacy workbook, plus update guides. See [docs/06-implementation-plan.md](docs/06-implementation-plan.md).

## Repository guide

| Path | Contents |
| --- | --- |
| `docs/` | The full case study, split into six short documents |
| `templates/` | CSV templates showing the standard raw data format for each department |
| `dashboard/` | The Excel workbook with the redesigned dashboard (illustrative data) |
| `projects/manufacturing-dashboard-prototype/` | A smaller earlier project: an Excel dashboard on a 60-month sample dataset |

## Skills shown

- Business process analysis: as-is mapping, pain-point discovery, to-be design
- Data standardization and data modeling for reporting
- Excel dashboards: pivot tables, slicers, structured tables, lookups, charts
- Option analysis with stated trade-offs, and change impact by role
- Stakeholder communication: iterated the design with the CX Analytics team and presented it twice
- Documentation and handover guides

## A note on the data

All workbooks and templates in this repository use anonymized, illustrative data. Customer names are replaced with placeholders and internal links, email addresses and file paths are removed.
