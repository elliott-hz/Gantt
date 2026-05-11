# Module 2: Usage Detection & Event Capture Engine

## C.2.1. Capture Usage Events

### C.2.1.1 Multi-modal Data Ingestion
- C.2.1.1.1 Road toll system data ingestion (gantry, toll tag transaction records)
- C.2.1.1.2 Public transport system data ingestion (train/bus tap-in/tap-out, transit card transactions)
- C.2.1.1.3 Road usage data ingestion (GPS telemetry, smart road sensors, heavy vehicle scheme records)
- C.2.1.1.4 Parking system data ingestion (meter, digital parking sensor entry/exit logs)
- C.2.1.1.5 Shared mobility service data ingestion (car-share/e-bike provider API consumption)
- C.2.1.1.6 Vehicle registration & identity source data ingestion

### C.2.1.2 Data Standardization & Normalization
- C.2.1.2.1 Iteration 1: Heterogeneous data format unification across all transport systems
- C.2.1.2.2 Iteration 1: Cross-system schema normalization to resolve structural incompatibilities
- C.2.1.2.3 Iteration 1: Unified data layer creation for downstream processing

---

## C.2.2. Validate Event Authenticity

### C.2.2.1 Identity & Integrity Validation (Iteration 1 Base Functionality)
- C.2.2.1.1 Cross-check against Module 1 Authorized Device Identity Whitelist
- C.2.1.2 Fraud rule base validation (duplicate event, location spoofing, anomaly detection)
- C.2.2.1.3 Invalid/fraudulent usage event blocking

### C.2.2.2 Suspicious Activity Handling (Iteration 1 Base Functionality)
- C.2.2.2.1 High-risk event alert triggering
- C.2.2.2.2 Fraud event alarm data logging for compliance and customer support

### C.2.2.3 Functionality Enhancement
- C.2.2.3.1 Iteration 2: Advanced fraud detection rule enhancement
- C.2.2.3.2 Iteration 3: Real-time anomaly detection capability enhancement
- C.2.2.3.3 Iteration 4: Machine learning-based fraud prediction enhancement

---

## C.2.3. Timestamp & Geo-tag Movement

### C.2.3.1 Event Structured Processing (Iteration 1 Base Functionality)
- C.2.3.1.1 Raw unstructured event data transformation into machine-readable standardized records
- C.2.3.1.2 Consistent timestamping of each usage event
- C.2.3.1.3 Precise geotagging of each usage event
- C.2.3.1.4 User/vehicle identifier tagging for each event
- C.2.3.1.5 Transport mode classification tagging (private vehicle / public transit / shared mobility / parking / toll)

### C.2.3.2 Trip & Route Analysis (Iteration 1 Base Functionality)
- C.2.3.2.1 Individual event aggregation into complete end-to-end trips
- C.2.3.2.2 Travel route reconstruction with origin/destination tagging
- C.2.3.2.3 Trip context enrichment (congestion zones, time-of-day segments, zone-based pricing context)
- C.2.3.2.4 Trip-level dataset generation for pricing accuracy

### C.2.3.3 Functionality Enhancement
- C.2.3.3.1 Iteration 2: Enhanced geospatial accuracy and real-time processing
- C.2.3.3.2 Iteration 3: Advanced trip pattern recognition and multi-modal journey stitching
- C.2.3.3.3 Iteration 4: Predictive trip analysis and dynamic route optimization

---

## C.2.4. Send Structured Events to Pricing Engine (P5: Data Synchronization Process)

### C.2.4.1 Downstream System Data Distribution (Iteration 1 Base Functionality)
- C.2.4.1.1 Real-time structured event data sync to Module 3 Dynamic Pricing Engine (via Kafka broker)
- C.2.4.1.2 Structured trip data sync to Module 5 Analytics & Planning Module
- C.2.4.1.3 Structured event/trip data batch/real-time sync to Snowflake Data Warehouse & BI

### C.2.4.2 Cross-System Consistency & Workflow Support (Iteration 1 Base Functionality)
- C.2.4.2.1 Data consistency maintenance across pricing, billing, and analytics workflows
- C.2.4.2.2 Fraud event data integration with Zendesk customer support ticketing workflows

### C.2.4.3 Functionality Enhancement
- C.2.4.3.1 Iteration 2: Enhanced data synchronization reliability and error handling
- C.2.4.3.2 Iteration 3: Advanced workflow orchestration and cross-system data governance
- C.2.4.3.3 Iteration 4: Real-time analytics pipeline integration and automated data quality monitoring

---

## A. Requirements Analysis
- A.1 Functional requirements gathering and documentation
  - A.1.1 Iteration 1 requirements analysis
  - A.1.2 Iteration 2 requirements analysis
  - A.1.3 Iteration 3 requirements analysis
  - A.1.4 Iteration 4 requirements analysis
- A.2 Non-functional requirements specification
  - A.2.1 Iteration 1 non-functional requirements
  - A.2.2 Iteration 2 non-functional requirements
  - A.2.3 Iteration 3 non-functional requirements
  - A.2.4 Iteration 4 non-functional requirements
- A.3 Stakeholder review and approval
  - A.3.1 Iteration 1 stakeholder review
  - A.3.2 Iteration 2 stakeholder review
  - A.3.3 Iteration 3 stakeholder review
  - A.3.4 Iteration 4 stakeholder review

---

## B. Product and System Design
- B.1 System architecture design
  - B.1.1 Iteration 1 architecture design
  - B.1.2 Iteration 2 architecture design
  - B.1.3 Iteration 3 architecture design
  - B.1.4 Iteration 4 architecture design
- B.2 Data flow and interface design
  - B.2.1 Iteration 1 data flow design
  - B.2.2 Iteration 2 data flow design
  - B.2.3 Iteration 3 data flow design
  - B.2.4 Iteration 4 data flow design
- B.3 Security and compliance design
  - B.3.1 Iteration 1 security design
  - B.3.2 Iteration 2 security design
  - B.3.3 Iteration 3 security design
  - B.3.4 Iteration 4 security design

---

## D. System Testing
- D.1 Test plan development
  - D.1.1 Iteration 1 test plan
  - D.1.2 Iteration 2 test plan
  - D.1.3 Iteration 3 test plan
  - D.1.4 Iteration 4 test plan
- D.2 Integration and end-to-end testing
  - D.2.1 Iteration 1 integration testing
  - D.2.2 Iteration 2 integration testing
  - D.2.3 Iteration 3 integration testing
  - D.2.4 Iteration 4 integration testing
- D.3 Performance and security testing
  - D.3.1 Iteration 1 performance testing
  - D.3.2 Iteration 2 performance testing
  - D.3.3 Iteration 3 performance testing
  - D.3.4 Iteration 4 performance testing

---

## E. System Delivery
- E.1 System deployment, release management, and operational handover
  - E.1.1 Iteration 1 deployment and release
  - E.1.2 Iteration 2 deployment and release
  - E.1.3 Iteration 3 deployment and release
  - E.1.4 Iteration 4 deployment and release