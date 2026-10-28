# 6. Implementation plan

## Decision for each sheet in the legacy workbook

Every existing sheet received one of four decisions, and the new sheets were listed for addition.

| Action | Sheets | Reason |
| --- | --- | --- |
| Retain (6) | `GUIDE`, `TICKET REPORT`, `TICKET DETAILS`, `REJECT REPORT`, `SLA REPORT`, `PVT_SLA` | Still useful as they are |
| Hide (4) | `MAIN`, `2024`, `2025`, `YOY` | Kept for reference, replaced by the new dashboard |
| Adjust (2) | `PENDING PROD`, `PENDING PERSO` | Reshape to the standard format |
| Remove (10) | Old pivot sheets and raw lists such as `PVOT`, `PVT PO`, `PENDING PO`, `PVT PROD`, `PVT PERSO`, `PENDING UMID`, `REJECT DETAILS`, `PERSO REJECT` and others | Their job moves to the new raw sheets and dashboard pivots |
| Add (13) | `PROPOSED DASHBOARD`, `DASHBOARD_DATA`, `DASHBOARD PIVOT TABLES`, plus the raw data sheets for production, purchase orders, UMID, personalization, output, compliance and quality | The new structure |

## Progress at submission (Aug 29, 2025)

| Work item | Status |
| --- | --- |
| Dashboard V1 and V2 prototypes | Completed |
| Dashboard V3 with team feedback | Completed |
| Standardized raw data format | Completed |
| Documentation of dashboard logic and data standard | Completed |
| Feasibility of a Power BI transition | Completed |
| Research for an SLA dashboard | Ongoing |
| Gradual transition to the proposed report | Ongoing |
| Go or no-go decision on adoption | Pending approval |

## Handover material

- Update guide for each raw data sheet
- Slicer guide for dashboard users
- Glossary of report terms
- Folder structure and dashboard logic notes
