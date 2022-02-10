# Project Title

This is the Solidity Kasei Coin minting application for Challenge 21! I'm a decentralized central federal reserve bank in this one in a manner of speaking!  I begin by creating a KaseiCoin token contract. I import ERC20, ERC20Detailed, and ERC20Mintable libraries so I can inherit from them.  I create a constructor where I define name, symbol, and the initial supply of coins I will initially create when I deploy the contract. In my case in the video I did one million (1,000,000) Kasei Coins.
I create another constructor this time calling on the ERC20Detailed library where I pass the parameters name, symbol, and 18
to signify the wei currency decimal places parameter.

After the above is complete I create a KaseiCoinCrowdsale contract that inherits from Crowdsale and MintedCrowdsale OpenZeppelin contracts.  I create a constructor that has the parameters rate, wallet, and coin in my case. This coin is the KaseiCoin that KaseiCoinCrowdsale will actually be using.  

The final piece is the deployer contract.  I create variables that store the addresses of the KaseiCoin and KaseiCoinCrowdsale contracts.  I instantiate a new instance of a KaseiCoin with params name, symbol, and an initial supply of 0.  I then assign the KaseiCoin contracts address to the kasei_coin_address variable.  I now instantiate a new instance of the KaseiCoinCrowdsale contract with params equal to a rate of 1, wallet, and coin. I assign the KaseiCoinCrowdsale contract's address to the kasei_crowdsale_address.  I make this contract a minter, and I renounce the minter role from the KaseiCoinCrowdsaleDeployer.

That's it!



## Technologies

I am using python version 3.7.10.  I go to the website https://remix.ethereum.org/ and run joint_savings.sol on the webpage and that's it.

-----

## Installation Guide

I have python version 3.7.10 and git version 2.33.0.windows.2 installed on a laptop running windows 10 pro.
---


## Usage

go to the website https://remix.ethereum.org/ and run both KaseiCoin.sol and KaseiCoinCrowdsale.sol on the webpage and that's it. The user needs to compile the code and then deploy it, and you should be able to test all the functions as needed.

---

## Contributors
Just me, Paul Lopez.

---

## License
No licenses required. Just install everything for free, pull from my repository, and enjoy!
