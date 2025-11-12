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


