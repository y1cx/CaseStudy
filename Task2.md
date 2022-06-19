
## Task 2 : Innovative ideas

Context : In Supply Chain process, a company should rely on their suppliers. However, some of your suppliers have made some mistakes in the delivery (missing or wrong items shipped) and the production has been stopped. As a Data Scientist, working in a famous Food Company, your manager asks you to detect bad suppliers. Give some ideas to solves this problem. 

Leading points : 

1) Explain the process/methodology/models and justify it.
2) What kind of data do you need to solve this problem ? 
3) What are the limits of your ideas ?


Hint : 
- The level of escalation can be measure according the some features : Missing and wrong items at the delivery, Delays...
- Bad suppliers are not a majority of the suppliers. 


### Solutions

1) The process / methodology / model

For the detection of bad suppliers in a food company, the historical supply, and delivery data are required for the problem. The model's output is supplier reliability score, which could be affected by the delayed delivery, less amount of products delivered than required, amount of the wrong items delivered, amount of poor quality of the item delivered, and the return of items due to wrong delivery or poor quality. As most deliveries meet the standards, and most suppliers are chosen are good suppliers, they should have similar patterns and higher reliability, while bad suppliers have more abnormal deliveries. 

The state-of-the-art anomaly detection models can be applied, e.g., Autoencoder, which is trained to reconstruct features of good suppliers, will manifest larger reconstruction errors for bad suppliers.

A supplier is labeled as the bad supplier with the comparison of the score predicted by the model and a baseline of reliability score.

2) Data

The historical supply and delivery data which has the following features:
* supplier name
* location
* shipment mode
* scheduled delivery date 
* recorded delivery date (delays)
* item brand
* item name
* required amount of item
* delivered amount of item (missing items)
* item price
* confirmed amount of item
* delivered amount of the wrong item
* returned amount of item (wrong items or items with poor quality))

3) Limits

The class imbalance problem could occur, as the majority of deliveries are good, and bad deliveries, and suppliers are the minority. Although anomaly detection models could be more effective than binary classification when dealing with unbalanced data, their stability still depends highly on the degree of imbalance.

The labeled historical data with qualified deliveries could be difficult to obtain, although a majority of suppliers are good suppliers.

External factors could affect the deliveries and could be further investigated as well, like the weather condition, the transport condition, and special events (e.g., festivals, pandemics, military situations).
