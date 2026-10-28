# Raw data templates

Header rows for the standard raw data format, each with a few fictional example rows. Customer names are placeholders.

| File | Used for |
| --- | --- |
| `dispatch_raw.csv` | Cards delivered to clients |
| `perso_received_raw.csv` | Personalization jobs received |
| `perso_pending_raw.csv` | Personalization jobs still pending |
| `output_fulfillment_raw.csv` | Cards kitted by fulfillment |
| `output_embedding_raw.csv` | Cards processed in embedding |
| `po_received_raw.csv` | Purchase orders received |
| `compliance_raw.csv` | Incident reports by department |

Rules: one row per transaction, dates as YYYY-MM-DD, quantities as whole numbers, client type and scheme taken from the lookup list.
