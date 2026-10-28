# 1. Problem and legacy process

## Context

The Daily Plant Report summarizes five areas of plant activity: Production, Personalization, Dispatch, Output and Compliance. It is due at 11:00 AM each day. Before this project it was produced by one or two analysts following a 22-page procedure with 32 manual steps, then sent out as static tables.

## Problem

- The process was error-prone and slow. Each step meant opening a different file, copying a range and pasting it into the summary workbook.
- Departments used different formats, so the same kind of information had to be reshaped before it could be combined.
- The report depended on a few people finishing on time, and it was delayed whenever a source file arrived late.
- Accountability was unclear. One person consolidated everything, so an incorrect figure could not easily be traced to its source.
- The static output could not be filtered, so decision-makers could not look at a single month or client type.

## Pain points reported by the team

1. Repetitive, tiring encoding steps
2. Difficulty aligning formats across departments
3. No standardization of raw data
4. Static tables when sending reports

## Legacy process by group

The 32 steps fall into twelve groups. Time per day is my estimate from walking through the procedure.

| Group | Legacy steps | What happened |
| --- | --- | --- |
| Gathering files | 1 | Download the day's files from a shared folder |
| Production data | 2 to 5 | Copy received jobs, balances and output from the production weekly report |
| Dispatch data | 6 to 7 | Copy delivery quantities per type from the delivery file |
| Compliance data | 8 to 9 | Filter external reports and count them by department |
| Quality assurance data | 10 to 12 | Copy inspected and reject counts per defect category, plus QA output |
| Output: embedding | 13 to 15 | Add a month column, build a pivot, copy quantities across |
| Output: fulfillment | 16 to 18 | Same method as embedding, from the fulfillment file |
| Personalization: received | 19 to 23 | Consolidate several summary files, tag each customer by type, pivot, copy |
| Personalization: pending | 24 to 29 | Filter pending statuses, tag, pivot, copy |
| Personalization: UMID | 30 | Add a month column, pivot by status, copy |
| Purchase orders | 31 | Rebuild the pending purchase order view |
| Finalization | 32 | Save to the shared folder using the naming convention and send to recipients |

The same hand-built pivot (add a month column, put month in rows, sum the quantity, copy the result) appears in at least five different places. That repetition was the clearest sign the raw data needed one standard layout.
