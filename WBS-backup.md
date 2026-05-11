# Module 2: Usage Detection & Event Capture Engine

## M2-1. Capture Usage Events

### M2-1.1 Multi-modal Data Ingestion
- M2-1.1.1 Road toll system data ingestion (gantry, toll tag transaction records)
- M2-1.1.2 Public transport system data ingestion (train/bus tap-in/tap-out, transit card transactions)
- M2-1.1.3 Road usage data ingestion (GPS telemetry, smart road sensors, heavy vehicle scheme records)
- M2-1.1.4 Parking system data ingestion (meter, digital parking sensor entry/exit logs)
- M2-1.1.5 Shared mobility service data ingestion (car-share/e-bike provider API consumption)
- M2-1.1.6 Vehicle registration & identity source data ingestion

### M2-1.2 Data Standardization & Normalization
- M2-1.2.1 Iteration 1: Heterogeneous data format unification across all transport systems
- M2-1.2.2 Iteration 1: Cross-system schema normalization to resolve structural incompatibilities
- M2-1.2.3 Iteration 1: Unified data layer creation for downstream processing

---

## M2-2. Validate Event Authenticity

### M2-2.1 Identity & Integrity Validation (Iteration 1 Base Functionality)
- M2-2.1.1 Cross-check against Module 1 Authorized Device Identity Whitelist
- M2.1.2 Fraud rule base validation (duplicate event, location spoofing, anomaly detection)
- M2-2.1.3 Invalid/fraudulent usage event blocking

### M2-2.2 Suspicious Activity Handling (Iteration 1 Base Functionality)
- M2-2.2.1 High-risk event alert triggering
- M2-2.2.2 Fraud event alarm data logging for compliance and customer support

### M2-2.3 Functionality Enhancement
- M2-2.3.1 Iteration 2: Advanced fraud detection rule enhancement
- M2-2.3.2 Iteration 3: Real-time anomaly detection capability enhancement
- M2-2.3.3 Iteration 4: Machine learning-based fraud prediction enhancement

---

## M2-3. Timestamp & Geo-tag Movement

### M2-3.1 Event Structured Processing (Iteration 1 Base Functionality)
- M2-3.1.1 Raw unstructured event data transformation into machine-readable standardized records
- M2-3.1.2 Consistent timestamping of each usage event
- M2-3.1.3 Precise geotagging of each usage event
- M2-3.1.4 User/vehicle identifier tagging for each event
- M2-3.1.5 Transport mode classification tagging (private vehicle / public transit / shared mobility / parking / toll)

### M2-3.2 Trip & Route Analysis (Iteration 1 Base Functionality)
- M2-3.2.1 Individual event aggregation into complete end-to-end trips
- M2-3.2.2 Travel route reconstruction with origin/destination tagging
- M2-3.2.3 Trip context enrichment (congestion zones, time-of-day segments, zone-based pricing context)
- M2-3.2.4 Trip-level dataset generation for pricing accuracy

### M2-3.3 Functionality Enhancement
- M2-3.3.1 Iteration 2: Enhanced geospatial accuracy and real-time processing
- M2-3.3.2 Iteration 3: Advanced trip pattern recognition and multi-modal journey stitching
- M2-3.3.3 Iteration 4: Predictive trip analysis and dynamic route optimization

---

## M2-4. Send Structured Events to Pricing Engine (P5: Data Synchronization Process)

### M2-4.1 Downstream System Data Distribution (Iteration 1 Base Functionality)
- M2-4.1.1 Real-time structured event data sync to Module 3 Dynamic Pricing Engine (via Kafka broker)
- M2-4.1.2 Structured trip data sync to Module 5 Analytics & Planning Module
- M2-4.1.3 Structured event/trip data batch/real-time sync to Snowflake Data Warehouse & BI

### M2-4.2 Cross-System Consistency & Workflow Support (Iteration 1 Base Functionality)
- M2-4.2.1 Data consistency maintenance across pricing, billing, and analytics workflows
- M2-4.2.2 Fraud event data integration with Zendesk customer support ticketing workflows

### M2-4.3 Functionality Enhancement
- M2-4.3.1 Iteration 2: Enhanced data synchronization reliability and error handling
- M2-4.3.2 Iteration 3: Advanced workflow orchestration and cross-system data governance
- M2-4.3.3 Iteration 4: Real-time analytics pipeline integration and automated data quality monitoring

---

## M2-5. Requirements Analysis
- M2-5.1 Functional requirements gathering and documentation
  - M2-5.1.1 Iteration 1 requirements analysis
  - M2-5.1.2 Iteration 2 requirements analysis
  - M2-5.1.3 Iteration 3 requirements analysis
  - M2-5.1.4 Iteration 4 requirements analysis
- M2-5.2 Non-functional requirements specification
  - M2-5.2.1 Iteration 1 non-functional requirements
  - M2-5.2.2 Iteration 2 non-functional requirements
  - M2-5.2.3 Iteration 3 non-functional requirements
  - M2-5.2.4 Iteration 4 non-functional requirements
- M2-5.3 Stakeholder review and approval
  - M2-5.3.1 Iteration 1 stakeholder review
  - M2-5.3.2 Iteration 2 stakeholder review
  - M2-5.3.3 Iteration 3 stakeholder review
  - M2-5.3.4 Iteration 4 stakeholder review

---

## M2-6. Product and System Design
- M2-6.1 System architecture design
  - M2-6.1.1 Iteration 1 architecture design
  - M2-6.1.2 Iteration 2 architecture design
  - M2-6.1.3 Iteration 3 architecture design
  - M2-6.1.4 Iteration 4 architecture design
- M2-6.2 Data flow and interface design
  - M2-6.2.1 Iteration 1 data flow design
  - M2-6.2.2 Iteration 2 data flow design
  - M2-6.2.3 Iteration 3 data flow design
  - M2-6.2.4 Iteration 4 data flow design
- M2-6.3 Security and compliance design
  - M2-6.3.1 Iteration 1 security design
  - M2-6.3.2 Iteration 2 security design
  - M2-6.3.3 Iteration 3 security design
  - M2-6.3.4 Iteration 4 security design

---

## M2-7. System Testing
- M2-7.1 Test plan development
  - M2-7.1.1 Iteration 1 test plan
  - M2-7.1.2 Iteration 2 test plan
  - M2-7.1.3 Iteration 3 test plan
  - M2-7.1.4 Iteration 4 test plan
- M2-7.2 Integration and end-to-end testing
  - M2-7.2.1 Iteration 1 integration testing
  - M2-7.2.2 Iteration 2 integration testing
  - M2-7.2.3 Iteration 3 integration testing
  - M2-7.2.4 Iteration 4 integration testing
- M2-7.3 Performance and security testing
  - M2-7.3.1 Iteration 1 performance testing
  - M2-7.3.2 Iteration 2 performance testing
  - M2-7.3.3 Iteration 3 performance testing
  - M2-7.3.4 Iteration 4 performance testing

---

## M2-8. System Delivery
- M2-8.1 System deployment, release management, and operational handover
  - M2-8.1.1 Iteration 1 deployment and release
  - M2-8.1.2 Iteration 2 deployment and release
  - M2-8.1.3 Iteration 3 deployment and release
  - M2-8.1.4 Iteration 4 deployment and release