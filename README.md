# Transaction Efficiency, Risk & Network Performance Overview – Lead Bank

**Author:** Loretta Chimezie   
**Date:** 2025-11-28

--- 

## Project Background
Lead Bank is experiencing a drop in transaction approvals which may be caused by internal banking issues or external network connectivity problems; recently upgraded fraud detection system which detects fraud but do not block it effectively; heavily invested 5G network slicing performance and app prioritization. This project analyzes available transaction data and produces an interactive Excel dashboard with actionable recommendations.



## Project Objective
1.	Transaction demographics – total number of transactions, average transaction amount, average latency(ms), total amount, average bandwidth
2.	Customer behavior – why are transfers failing? Identify the cause
3.	Network performance – identify the best network slice that impacts speed and smooth transactions
4.	Transaction trends – what time of day do we have transaction hike? Which network contributes to it? what other factors increases/decreases transactions
5.	App prioritization – analyze channel distribution (desktop vs mobile)
6.	Fraud leakages – why are the fraud detected transactions successful? Where is the problem coming from?



## Datasets
- **Transaction Overview.xlsx** — Transaction ID, Sender Account ID, Receiver Account ID, Transaction Amount



## Dashboard Features
- Key KPIs: Total Transactions, Total Amount, Avg. Latency, Avg. Bandwidth, Average Amount
- Visuals: app distribution, time-series of transactions, transaction type breakdown, network slice chart, fraud flag 
- Interactivity: slicers/filters for network slice, fraud flag, transaction status, transaction type 



## Key Findings 
-	Slice 1 is efficient for mobile-app transfers, with 76 ms latency and an 80% success rate. It performs consistently all day and detects more fraud in deposit transactions.
-	Slice 2 performs well for withdrawals and desktop-app transactions, with 77 ms latency, an 80% success rate, and strong fraud detection for transfers.
-	There are high fraud leakages using the Slice 1 network with average latency of 77ms for transfers on the mobile app
-	Failed transactions occur more when using the desktop channel with Slice 1 network
-	Slice 3 network has the highest bandwidth
-	Fraud detected transfers are successful on the mobile device using Slice 1 network
-	Slice 2 generates more income due to the high rate of successful transactions
-	The mobile and desktop devices are both efficient
-	The time of day has little effect on the transaction status



## Recommendations
1.	Slice 1 and 2 networks are both good depending on which task its performing;
-	Slice 1 works fine for transfers on the mobile app 
-	For withdrawal using the desktop channel, Slice 2 is your plug
2.	For more successful transactions use the Slice 2 network on the mobile device
3.	Don’t encourage transactions on the mobile device when using Slice 1 as there’s high chances of fraud leakages
4.	Both desktop and mobile devices works well
5.	Navigate between networks where necessary
6.	Upgrade on the detection machine should be carried out again as soon as possible



## Tools & Techniques 
- Microsoft Excel (Pivot Tables, Pivot Charts, Slicers)   
- Data cleaning and transformation in PowerQuery  
- Dashboard layout and visualization best practices   
- Basic descriptive analytics and KPI design



## Project Files (included) 
- ` Transaction overview.xlsx` — interactive dashboard file   
- `/transaction_dataset_JanToOct/` — raw data files used for analysis (xlsx)   
- `Presentation.pdf` — boardroom slide deck (11 slides)   
- `README.md` — this documentation



## How to Run / View 
1. Open `Transaction overview.xlsx` in Excel (desktop recommended)   
2. Enable content (if prompted) to allow Pivot Tables and slicers to work   
3. Use slicers to filter by Network Slice ID, Fraud flag, transaction status, etc.   
4. Refer to `Presentation.pdf` for a summary of insights and recommended actions



## Contact 
Loretta Chimezie   
Email: _chimezieloretta@gmail.com_    
LinkedIn: _ https://www.linkedin.com/in/loretta-chimezie/_
