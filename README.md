Crowdsale contract allows for creation and minting of ERC20 tocken PupperCoin inheriting OpenZepplin Solidity Library code 

Environment is Injected Web 3 interacts with Metamask wallet (in Google Chrome extension) bc Metamask will only interact with web 3 

Ropsten network is the test network to send and receive and store eths

Gas limit is determine by default 0 value 

In order to deplay the contract PupperCoinSaleDeployer is selected.  The goal is 300 Pupper (pup coins)


In (first) contract PupperCoinSale is Crowdsale, MintedCrowdsale, CappedCrowdsale, TimedCrowdsale, RefundablePostDeliveryCrowdsal
PuppercoinSale is the parent and the rest are children.  One main contract is inheriting the others.

The constructor is used to initialize state variables of a contract. In this case case we initializing variables- rate. wallet, goal, open, close, token with 
non negative integer

Then we are passing the constructor values to the crowdsale, keeping the contrac "public" with open documentation 

PuppercoinSaleDeployer contract deploys token_sale_address, which is the Metamask address and koen_address is my puppercoinaddress, 
which is initiated when puper coins created. 

Then the contract goes through initializing contractor parameters- goal, name, symbol, and wallet 

Next new coins are created using the name, symbol and keeping the supply parameter as 0)

Then we create PupperCoinSale P_sale variable where the "new" contract is actually the contract and it specifies the exchange rate of 1 to 1 eth
wallet (address), minting taking place now and 24 weeks from now, and passing through coin parameter)

Finally, the minting execution takes place to a token_sale_address and afterwards its end is defined by token.renounceMinter();

Please see the screenshots with code and transactions.