# WBS for Gantt Chart - Complete Project Breakdown

## Module 2: Usage Detection & Event Capture Engine (Functional)

| WBS | TASK | Predecessor | DAYS |
|-----|------|-------------|------|
| 1.1.1 | Road toll system data ingestion (gantry, toll tag transaction records) | - | 10 |
| 1.1.2 | Public transport system data ingestion (train/bus tap-in/tap-out, transit card transactions) | 1.1.1 | 10 |
| 1.1.3 | Road usage data ingestion (GPS telemetry, smart road sensors, heavy vehicle scheme records) | 1.1.2 | 10 |
| 1.1.4 | Parking system data ingestion (meter, digital parking sensor entry/exit logs) | 1.1.3 | 10 |
| 1.1.5 | Shared mobility service data ingestion (car-share/e-bike provider API consumption) | 1.1.4 | 10 |
| 1.1.6 | Vehicle registration & identity source data ingestion | 1.1.5 | 10 |
| 1.2.1 | Heterogeneous data format unification across all transport systems | 1.1.6 | 15 |
| 1.2.2 | Cross-system schema normalization to resolve structural incompatibilities | 1.2.1 | 15 |
| 1.2.3 | Unified data layer creation for downstream processing | 1.2.2 | 10 |
| 2.1.1 | Cross-check against Module 1 Authorized Device Identity Whitelist | 1.2.3 | 10 |
| 2.1.2 | Fraud rule base validation (duplicate event, location spoofing, anomaly detection) | 2.1.1 | 10 |
| 2.1.3 | Invalid/fraudulent usage event blocking | 2.1.2 | 5 |
| 2.2.1 | High-risk event alert triggering | 2.1.3 | 5 |
| 2.2.2 | Fraud event alarm data logging for compliance and customer support | 2.2.1 | 5 |
| 3.1.1 | Raw unstructured event data transformation into machine-readable standardized records | 2.2.2 | 10 |
| 3.1.2 | Consistent timestamping of each usage event | 3.1.1 | 5 |
| 3.1.3 | Precise geotagging of each usage event | 3.1.2 | 5 |
| 3.1.4 | User/vehicle identifier tagging for each event | 3.1.3 | 5 |
| 3.1.5 | Transport mode classification tagging (private vehicle / public transit / shared mobility / parking / toll) | 3.1.4 | 5 |
| 3.2.1 | Individual event aggregation into complete end-to-end trips | 3.1.5 | 10 |
| 3.2.2 | Travel route reconstruction with origin/destination tagging | 3.2.1 | 10 |
| 3.2.3 | Trip context enrichment (congestion zones, time-of-day segments, zone-based pricing context) | 3.2.2 | 10 |
| 3.2.4 | Trip-level dataset generation for pricing accuracy | 3.2.3 | 5 |
| 4.1.1 | Real-time structured event data sync to Module 3 Dynamic Pricing Engine (via Kafka broker) | 3.2.4 | 10 |
| 4.1.2 | Structured trip data sync to Module 5 Analytics & Planning Module | 4.1.1 | 10 |
| 4.1.3 | Structured event/trip data batch/real-time sync to Snowflake Data Warehouse & BI | 4.1.2 | 10 |
| 4.2.1 | Data consistency maintenance across pricing, billing, and analytics workflows | 4.1.3 | 5 |
| 4.2.2 | Fraud event data integration with Zendesk customer support ticketing workflows | 4.2.1 | 5 |

---

## Module 5: Requirements Management

| WBS | TASK | Predecessor | DAYS |
|-----|------|-------------|------|
| 5.1 | Gather stakeholder requirements | - | 10 |
| 5.2 | Define functional and non-functional requirements | 5.1 | 10 |
| 5.3 | Review and finalize requirements with stakeholders | 5.2 | 5 |
| 5.4 | Maintain requirements traceability matrix | 5.3 | 5 |

---

## Module 6: Project Testing

| WBS | TASK | Predecessor | DAYS |
|-----|------|-------------|------|
| 6.1 | Develop test strategy and plan | 4.2.2, 5.4 | 5 |
| 6.2 | Create test cases and scripts | 6.1 | 15 |
| 6.3 | Execute unit, integration, and system testing | 6.2 | 20 |
| 6.4 | Perform UAT with limited user groups | 6.3 | 10 |
| 6.5 | Report defects and track resolution | 6.4 | 10 |

---

## Module 7: Release and Operations

| WBS | TASK | Predecessor | DAYS |
|-----|------|-------------|------|
| 7.1 | Prepare deployment package and environment | 6.5 | 5 |
| 7.2 | Full-scale deployment to production | 7.1 | 5 |
| 7.3 | Conduct post-launch validation and compliance audit | 7.2 | 10 |
| 7.4 | Provide operator training and citizen onboarding | 7.3 | 10 |
| 7.5 | Offer post-launch support and stabilization | 7.4 | 20 |

---

## Notes

- **WBS 1-4**: Functional modules (Usage Detection & Event Capture Engine) - retained original 3-level hierarchy
- **WBS 5-7**: Project management phases - simplified to 2-level hierarchy
- **PROGRESS**: All tasks start at 0% (to be updated in Excel/Gantt tool)
- **START/END**: Auto-calculated based on project start date in Excel
- **Dependencies**: Logical flow maintained from data ingestion → processing → testing → deployment
