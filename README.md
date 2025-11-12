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
| Row 3    | Data 5   |

'SOLDTO', 'PLANT',
       'SHIPTO COUNTRY', 'ROUTE', 'MATERIAL', 'SHIPPING CONDITION',
       'SHIPPING TYPE', 'CS REGION', 'INCOTERM', 'MODALITY',
       'REQUESTED QUANTITY', 'PAYER', 'PAYMENT TERM', 'ORDER TYPE',
       'SALES OFFICE', 'SALES UNIT', 'SHIPTO', 'SHIPPING POINT',
       'DCHAIN STATUS', 'CREATED BY', 'WEIGHT UNIT', 'DAYSLEFT RDD VS PLAN GI',
       'DAYSLEFT RDD VS RDD', 'DAYSLEFT TPT VS PLAN GI', 'DAYSLEFT TPT VS RDD',
       'DAYSLEFT MAT AVAIL VS PLAN GI', 'DAYSLEFT MAT AVAIL VS RDD',
       'DAYSLEFT CONFIRM GI DATE  VS PLAN GI',
       'DAYSLEFT CONFIRM GI DATE VS RDD', 'DAYSLEFT CREDIT HOLD VS PLAN GI',
       'DAYSLEFT CREDIT HOLD VS RDD', 'CREDIT HOLD OCCURENCCE',
       'DAYSLEFT DELIVERY BLOCK VS PLAN GI', 'DAYSLEFT DELIVERY BLOCK VS RDD',
       'DAYSLEFT INCO VS PLAN GI', 'DAYSLEFT INCO VS RDD',
       'DAYSLEFT ROUTE VS PLAN GI', 'DAYSLEFT ROUTE VS RDD',
       'DAYSLEFT SHIPTO VS PLAN GI', 'DAYSLEFT SHIPTO VS RDD',
       'DAYSLEFT SHIPPING POINT VS PLAN GI', 'DAYSLEFT SHIPPING POINT VS RDD',
       'DAYSLEFT SHIPPING TYPE  VS PLAN GI', 'DAYSLEFT SHIPPING TYPE VS RDD',
       'THROUGHPUT  CREATE VS CONF', 'THROUGHPUT  CONF VS DEL',
       'THROUGHPUT DEL VS GI', 'VBAPROUTE_IN_DAYS', 'PLAN GI DATE', 'TPT',
       'ACTUAL GI DATE', 'RDD', 'SEA TOLERANCE', 'RAIL TOLERANCE',
       'IN FULL TOLERANCE'
