# 2. Standard raw data format

## Principle

Each department enters or exports its figures into a predefined table with the same header style, the same units and consistent categories. The format is modeled on the existing dispatch data, which already followed this shape.

## Rules

- One row per transaction
- One uniform header row
- Core fields present wherever they apply: date, month, customer or project name, client type, quantity
- Categories such as client type and card scheme come from a lookup table, not free text
- Each department has its own sheet, so an error traces back to one place

## Why it matters

In the legacy flow, a spelling difference such as two ways of writing the same card scheme would split one category into two in a pivot table. A lookup-driven standard prevents that, and it also means a pivot table or a Power BI model can read every sheet the same way.

## Raw data sheets in the redesigned workbook

| Sheet | Fields |
| --- | --- |
| `DISPATCH_RAW` | Month, Month name, Type, Project name, Delivered qty, Card type, Scheme |
| `PERSO_RECEIVED_RAW` | Date, Month, Type, Customer name, Quantity, Project |
| `PERSO_PENDING_RAW` | Date received, Month, Type, Company name, Qty |
| `UMID_PENDING_RAW` | Card holder, Status, Month, Date and time |
| `OUTPUT_FULFILLMENT_RAW` | Date, Month, Customer, Quantity transferred |
| `OUTPUT_EMBEDDING_RAW` | Date and time, Month, Project name, Category, Transfer qty |
| `PO_RECEIVED_RAW` | Date PO received, Month, Client, Category, PO qty, Subgroup, Balance |
| `COMPLIANCE_RAW` | Month, Customer, Complaint qty, Type, Department |
| `PROD_RECEIVED_RAW` | Month, then quantity per client type and a total |
| `PROD_PENDING_RAW` | Year or date received, Number of job orders, Number of cards, then quantity per client type |
| `QUALITY_RAW` | Monthly inspected and reject counts per defect category |
| `LOOKUP` | Customer to bank type, customer to scheme, project to type, client to type |

Ready-to-use templates for most of these are in [`templates/`](../templates/).

## Updating a raw data sheet

Each sheet has a short update guide: open the source file, copy only the listed columns, and paste them into the matching raw data sheet. Monthly sheets such as fulfillment and embedding append the current month and delete the earlier entries for that month first, so rows are never duplicated.
