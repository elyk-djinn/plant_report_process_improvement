# 4. Dashboard design

## Goals

Clarity, interactivity, flexibility and a modular structure that is easy to update and ready for later automation.

## Structure of the workbook

The workbook separates three kinds of sheets, color-coded so a new user can tell them apart: report sheets, raw data sheets, and control sheets.

| Layer | Examples | Role |
| --- | --- | --- |
| Report | `DASHBOARD`, `LEGACY DASHBOARD`, `YOY`, `TICKET REPORT` | What readers look at |
| Control | `DASHBOARD_DATA`, `DASHBOARD PIVOT TABLES`, `LOOKUP` | Calculations and pivot tables that feed the report |
| Raw data | `*_RAW` sheets | Pasted system exports in the standard format |

Refreshing the data connections updates the dashboard. Moving scorecards and text boxes changes the layout without touching the data.

## What the dashboard shows

- Pending purchase orders, total dispatch, total rejects and reject rate, each with a year-over-year comparison
- Total output, pending production and pending personalization
- Dispatch split by client type, card type and scheme
- Slicers for month and client type

## Using the slicer

1. Find the slicer, the filter box on the dashboard.
2. Click a month or client type.
3. Hold Ctrl or Shift to select several.
4. To clear, click the clear-filter icon on the slicer or hold Ctrl and click the selection again.

## Glossary

A `GUIDE` sheet defines the report's terms, so every reader uses the same words.

| Term | Meaning |
| --- | --- |
| Received EF | Count of data files received from customers |
| Pending PO | Purchase orders from account management that still need a job order before the plant can print |
| Pending production | Job orders waiting in the production section, with reasons |
| Dispatch | Card quantity delivered to clients |
| Output | Card quantity produced or processed by a unit |
| Reject rate | Rejected cards over cards inspected |
| Compliance | Count of external incident reports investigated by the compliance unit |

## Iteration history

| Version | Focus |
| --- | --- |
| V1 and V2 | Working prototypes, presented twice |
| V3 | Integrated team feedback, aligned the visuals with the data, checked each visual against the decisions it supports |
