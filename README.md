# Crowdsale in Remix

### Rich Ripley 11-30-20

![Ethereum Crowdsale](https://miro.medium.com/max/1400/1*F2b3YwJUYiZKmPXw0Tz9ig.png)

---

# Objective: 
Create and delpoy a crowdsale with the Puppercoin token. This being done via Kovan (on Remix) with the help of Metamask. In order to do this we will need to create a ERC20 Token minted through Crowdsale, leveraging the OpenZeppelin Solidity library. This crowdsale contract will manage the entire process, allowing users to send ETH and get back PCD24 (PupperCoin). Our goal will be to launch a Crowdsale with a maximum output of 300 Ether. Lastly, in order to confirm that the crowdsale took place, we will need to use [etherscan](https://kovan.etherscan.io/) to check that the contract was successful and PCD24 was transferred. 

# Contracts: 
The 3 contracts we will be using to achieve this are:
    
    1 - PupperCoin
    2 - PupperCoinSale
    3 - PupperCoinSaleDeployer
    
*Please refer to the atached .sol files for the contract code.* 

# Process: 
- In order to successfully launch the Crowdsale, you will need to follow these easy steps:

        1 - Compile 'PupperCoin' and then 'Crowdsale' files
        2 - Deploy 'PupperCoinSaleDeployer' from the wallet address of your choosing
        3 - Deploy 'PupperCoinSale' contract using the 'token_sale_address' from your PupperCoinSaleDeployer
        4 - Deploy 'PupperCoin' contract using the 'token_address' from your PupperCoinSaleDeployer
        5 - 'buyTokens' from your 'PupperCoinSale' contract using your wallet address
        
*Throughout these steps, you should be able to track your account activity via Metamask and accept or reject transactions.*

# Outcome:
Once your contracts are deployed and you successfully launch your Crowdsale, you should be able to track your transaction details via [etherscan](https://kovan.etherscan.io/). Your completed crowdsale launch should look like the below - 

![Successful Crowdsale Launch](https://user-images.githubusercontent.com/65874272/100963282-484a9500-34e3-11eb-9632-311ad26a85eb.png)

![Successfully bought tokens](https://user-images.githubusercontent.com/65874272/100963376-74feac80-34e3-11eb-9f23-9606c6789fcf.png)

Above, you can see the successful deployment of our Crowdsale, and then below that, the completed purchase of our PCD24 Token. 

# Help:

For any issues with the Crowdsale launch, refer to the following documentation - 

 - [Crowdsale docs](https://docs.openzeppelin.com/contracts/2.x/crowdsales)
 - [Refundable Crowdsale docs](https://docs.openzeppelin.com/contracts/2.x/api/crowdsale#RefundableCrowdsale)
 - [OpenZeppelin Contract docs](https://docs.openzeppelin.com/contracts/2.x/)
 

