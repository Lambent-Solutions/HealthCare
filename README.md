# HealthCare


Ethereum Blockchain for Health Care 

INTRODUCTION
This PoC demonstrates the use of Ethereum blockchain in healthcare. open http://localhost:8080 login into dashboard you will be able to deploy patient name, DOB, Sex and condition into blockchain and fetch them.  

How to install (Ubuntu)

run a private geth node 
> geth --datadir /home/ubuntu/test/ --networkid 1234   --rpc --rpcapi web3,personal,admin,db,eth,net --rpcaddr 0.0.0.0 --rpcport 8545 --rpccorsdomain "*" console 2>> log

inside geth node start miner

> personal.newAccount("your password")      // you can create multiple accounts

> personal.unlockAccount(eth.accounts[0], "password")

> miner.start()                             // start mining ethereum NOTE without you wont be able to deploy contracts 

open another terminal 

> truffle migrate
> npm run dev 
