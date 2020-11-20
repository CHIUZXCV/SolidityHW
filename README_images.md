# Solidity Homework Steps

## Background

Your new startup has created its own Ethereum-compatible blockchain to help connect financial institutions, and the team wants to build smart contracts to automate some company finances to make everyone's lives easier, increase transparency, and to make accounting and auditing practically automatic!

Fortunately, you've been learning how to program smart contracts with Solidity! What you will be doing this assignment is creating a few `ProfitSplitter` contracts. These contracts will do several things:

* Pay your Associate-level employees quickly and easily.

* Distribute profits to different tiers of employees.

* Distribute company shares for employees in a "deferred equity incentive plan" automatically.

## Files

## Instructions

1. Make sure Ganache and Meta Max are downloaded. Meta Max will act as a brdige between Remix IDE and Ganache. 

2. For the level one exercise, Associate Profit splitter, open up the file in Remix. Some changes in the code need to be made; specifically creating employee variables, and dividing the amount of ETH to be sent by 33.33% to each associate.

3. Below is an image of the code with the appropriate changes.
![Associate Profit](Images/ap_1.png)

4. After making changes, compile the code. Next, go to "Deploy and Run Transactions". Here, you will begin the process of sending the ETH to your employees via Meta Max.

5. Change your environment to 'Injected Web3', make the value 10 ETH, and pick three wallet addresses from Ganache. For the first exercise, these wallet addresses were chosen;
     0x43AfBb1872b41FCC280a8309912e20b92E58905a
     0x5976a7EF8eAfbAB6F06A285DeAE7A6C0c7D55391
     0xeDB528Ec8b73AEedAEF56C5f54891eFFdb34172B

6. The image below shows that before the transaction occurs, these balances were 100 in Ganache, showing that there were no changes in the account prior. 
![Prior Associate Profit](Images/prior_sent.png)

7. Press Transact, and your Meta Max should send the balances to Ganache. The next image shows the balance within the appropriate wallet addresses.
![Post Associate Profit](Images/post_sent.png)

8. For the level two exercise, this was a Tiered Profit splitter based off of C-suite employees. The CEO will receive 60%, less senior will receive 25%, and the least senior will receive 15%.

9. Below, is an image of the code that reflects the requirements dictated by the sample code.
![Tiered Profit](Images/ap_2.png)

10. Copy step 4.

11. For this exercise, three different wallet addresses will be used to show the transaction. Again, the initial balance will be 100 to show that no transactions have occured.
    0x7D5093635384CE7e660A0f85F9D350A97F1d866c
    0x7f3E9E69095B7e57CC2f4bD8dae0aeAc9b9C488c
    0x21612DebBCB190842d5341E33AF88fAbe588c7E0

12. Below is an image of the pre sending of ETH through Meta Max
![Tiered Profit](Images/prior_sent_2.png) 

13. After compiling and deploying, the employees' wallet should show 106, 102.5, and 101.5 ETH reflecting the tiered profit structure. 
![Tiered Profit](Images/post_sent_2.png)

