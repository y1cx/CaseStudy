# CaseStudyDS
Case Study Data Scientist Position / Think-Tank

Here you can find the Case Study for the Data Scientist position of Think-Tank BMW Group. 
This Case Study is the opportinity for us to assess some skills you will need as a Data Scientist in our Team and to show us your capacity to come up with innovative ideas when you are confronted to new problems. 
You have been given a 4 day deadline to submit your results. Afterwards, you will have the opportunity to present and discuss your results to different members of our team for 10-15 min.

Note : If you have any ideas but you didn't implement it, please write it in your deposite. 


## Task 1 : Model building

Context :  You work in a Crypto startup and you want to identify malicious Ethereum addresses. Fortunately, you have found 3 interesting datasets :

- malicious_adresses : Dataset of malicious addresses with a comment explaining the reason of suspecting the adresses. 
- malicious_transactions : Transaction data related to malicious adresses.

            * acc_name : Malicious address involve in the transaction.
            * blockNumber : The block number that the transaction was included in.
            * timeStamp : The time that the block was mined in UTC.
            * hash : A unique identifier that can be used to locate a specific transaction.
            * nonce : The count of transactions sent out of the account. The number is initialized at 0 and is incremented by 1 for each transaction sent.
            * blockHash : A unique identifier of the block. 
            * transactionIndex : Index transaction.
            * from : The address that originally sent the transaction.
            * to : The address that the transaction is addressed to.
            * value : The amount of Ether included in the transaction.
            * gaz : The upper limit of how much computational work and storage the sender is willing to expend on the transaction.
            * gasPrice : The amount of Ether per unit of gas the user is willing to pay for the transaction, commonly denoted in a subunit of Ether known as Gwei. 1 Gwei = 1x10^-9 Ether.
            * isError : bolean indicate if an error occure during the transaction
            * txreceipt_status : status of the transaction, "1" means the transaction succeded, "0" means the transaction failed. 
            * input : Information that is passed to a smart contract when a transaction is sent to its address. However, if the transaction is creating a contract, the contract’s bytecode is placed in the input data field.
            * contractAdress : The contract adress related to the input.
            * cumulativeGas : Sum of gasUsed by this transaction and all preceding transactions in the same block.
            * gasUsed : The amount of computational work and storage used in the transaction.
            * confirmations : Block number that confirmed the transaction. 
            
- normal_transactions : Transaction data related to normal adresses.

Leading points :

1) Explore the datasets, if necessary clean them and keep the revelant features.
2) Analyze the addresses' behavior. What helpful statements can you make?  
3) Group the addresses in several categories based on their behavior. Justify your grouping decision. 
4) Given the different groups you have created, what would you advise the business to do?  
5) Train a prediction model that predicts maliciousness based on financial behavior. How good does your model perform? How would you tweak it?
4) Given the prediction you have created, what would you advise the business to do?  
 
Feel free to use your own methodology to solve this problem. 


## Task 2 : Innovative ideas

Context : In Supply Chain process, a company should rely on their suppliers. However, some of your suppliers have made some mistakes in the delivery (missing or wrong items shipped) and the production has been stopped. As a Data Scientist, working in a famous Food Company, your manager asks you to detect bad suppliers. Give some ideas to solves this problem. 

Leading points : 

1) Explain the process/methodology/models and justify it.
2) What kind of data do you need to solve this problem ? 
3) What are the limits of your ideas ?


Hint : 
- The level of escalation can be measure according the some features : Missing and wrong items at the delivery, Delays...
- Bad suppliers are not a majority of the suppliers. 


# Enjoy the task and blow our minds !

