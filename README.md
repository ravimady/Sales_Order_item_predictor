# Sales Order item Predictor

## Objective of the project :
Prediction model that predicts whether a sales order item will delay or not. In addition to this, it is also capable of providing the top 3 actionable insights using Shapely analysis. In any large corporations in the manufacturing sector, this type of tool can provide the Customer Sales Rep teawm with valuable insights on being able to understand those order-items that will delay and be able to action on them or atleast prioritise them.

## Data Ingestion :

Usually companies rely on Commercial databases based out of SQL. Data is extracted from SAP or any other system equivalent. For demonstration purposes, I will make a hypothetical training dataset and a hypothetical open order dataset.

## Feature list :

|  FIELD   |  DESCRIPTION |
|----------|----------|
|ID   |  Sales-Order item   |
| event date   | Date when an activity change happens   | 
| SOLD TO   | Customer Number   |
| PLANT     | Producing Plant   |
| SHIPTO COUNTRY |               |
| ROUTE||
| MATERIAL ||
|SHIPPING TYPE | Mode of Shipment(ROAD, SEA etc)|
| REGION ||
| INCOTERM | Contractual terms |
| DAYSLEFT RDD VS PLAN GI| daysleft from the requested delivery date to the planned goods issue date|
| DAYSLEFT MAT AVAIL VS RDD | daysleft from the material availabiity date change to the requested delivery date|
| DAYSLEFT CREDIT HOLD VS RDD | daysleft from the credit hold occurence to the requested delivery date |

## Days Left feature engineering :

### Event-Driven Metrics (DAYSLEFT Columns)

Definition: Difference in days between RDD and relevant milestone dates.

Columns:

DAYSLEFT MAT AVAIL VS RDD
DAYSLEFT CONFIRM GI DATE VS PLAN GI
DAYSLEFT CONFIRM GI DATE VS RDD
DAYSLEFT CREDIT HOLD VS PLAN GI
DAYSLEFT CREDIT HOLD VS RDD
DAYSLEFT DELIVERY BLOCK VS PLAN GI
DAYSLEFT DELIVERY BLOCK VS RDD
DAYSLEFT INCO VS PLAN GI
DAYSLEFT INCO VS RDD
DAYSLEFT ROUTE VS PLAN GI
DAYSLEFT ROUTE VS RDD
DAYSLEFT SHIPTO VS PLAN GI
DAYSLEFT SHIPTO VS RDD
DAYSLEFT SHIPPING POINT VS PLAN GI
DAYSLEFT SHIPPING POINT VS RDD
DAYSLEFT SHIPPING TYPE VS PLAN GI
DAYSLEFT SHIPPING TYPE VS RDD


Logic:

First event: All DAYSLEFT columns = RDD - Event Date.
Subsequent events: Only selected columns (4 per event) are recalculated; others retain previous values.

### Key Characteristics

Event-driven changes: Simulates real-world updates (e.g., material availability, GI date changes).
Temporal consistency: All event dates occur before RDD.
Rich categorical and numeric features: Suitable for classification, regression, and time-series analysis.
