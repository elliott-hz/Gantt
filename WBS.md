# Module 2: Usage Detection & Event Capture Engine

## 1. Capture Usage Events

### 1.1 Multi-modal Data Ingestion
- 1.1.1 Road toll system data ingestion (gantry, toll tag transaction records)
- 1.1.2 Public transport system data ingestion (train/bus tap-in/tap-out, transit card transactions)
- 1.1.3 Road usage data ingestion (GPS telemetry, smart road sensors, heavy vehicle scheme records)
- 1.1.4 Parking system data ingestion (meter, digital parking sensor entry/exit logs)
- 1.1.5 Shared mobility service data ingestion (car-share/e-bike provider API consumption)
- 1.1.6 Vehicle registration & identity source data ingestion

### 1.2 Data Standardization & Normalization
- 1.2.1 Heterogeneous data format unification across all transport systems
- 1.2.2 Cross-system schema normalization to resolve structural incompatibilities
- 1.2.3 Unified data layer creation for downstream processing

---

## 2. Validate Event Authenticity

### 2.1 Identity & Integrity Validation
- 2.1.1 Cross-check against Module 1 Authorized Device Identity Whitelist
- 2.1.2 Fraud rule base validation (duplicate event, location spoofing, anomaly detection)
- 2.1.3 Invalid/fraudulent usage event blocking

### 2.2 Suspicious Activity Handling
- 2.2.1 High-risk event alert triggering
- 2.2.2 Fraud event alarm data logging for compliance and customer support

---

## 3. Timestamp & Geo-tag Movement

### 3.1 Event Structured Processing
- 3.1.1 Raw unstructured event data transformation into machine-readable standardized records
- 3.1.2 Consistent timestamping of each usage event
- 3.1.3 Precise geotagging of each usage event
- 3.1.4 User/vehicle identifier tagging for each event
- 3.1.5 Transport mode classification tagging (private vehicle / public transit / shared mobility / parking / toll)

### 3.2 Trip & Route Analysis
- 3.2.1 Individual event aggregation into complete end-to-end trips
- 3.2.2 Travel route reconstruction with origin/destination tagging
- 3.2.3 Trip context enrichment (congestion zones, time-of-day segments, zone-based pricing context)
- 3.2.4 Trip-level dataset generation for pricing accuracy

---

## 4. Send Structured Events to Pricing Engine (P5: Data Synchronization Process)

### 4.1 Downstream System Data Distribution
- 4.1.1 Real-time structured event data sync to Module 3 Dynamic Pricing Engine (via Kafka broker)
- 4.1.2 Structured trip data sync to Module 5 Analytics & Planning Module
- 4.1.3 Structured event/trip data batch/real-time sync to Snowflake Data Warehouse & BI

### 4.2 Cross-System Consistency & Workflow Support
- 4.2.1 Data consistency maintenance across pricing, billing, and analytics workflows
- 4.2.2 Fraud event data integration with Zendesk customer support ticketing workflows