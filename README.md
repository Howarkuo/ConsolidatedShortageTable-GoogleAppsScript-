# ConsolidatedShortageTable-GoogleAppsScript
## Aim:
- Fetch Batch Q:AP
- Single Active Cell Logging
- Column F Parsing 
- Daily / Weekly / Overhead Matching 
- Adjusted-Current Calculation 

### Overall Flow
```
Read:
    Current Inventory Value / Balance for each date range
    +
    Previous Inventory Values
    +
    Initial Stock ( L + M+ N)
    +
    Column F planned quantities
    
↓
Calculate Movement (xValue)
↓
Write one record into Movements:
(Date, Item No, Movement)

Current = Current + Column F Qty
Movement = Current - Previous
```
