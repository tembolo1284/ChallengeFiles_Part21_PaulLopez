# Project Title

This is the Solidity Smart Contract application for Challenge 20! So frightening how powerful this is!  I begin by creating
a withdraw() function that checks that the recipient is either AccountOne or AccountTwo. If the recipient is neither one I quit and 
alert the user with a message that they don't own the account. Most importantly from my perspective, I don't waste any gas because I used the require() function to do this!  Another check I do is that balance must be greater than or equal to the amount that the user wants to withdraw. If it isn't I display the message "Insufficient funds!".  I also make the lastToWithdraw variable set to the recipient if it isn't already.

I also create a deposit() function that allows a user to put money into the account.  This is pretty straightforward and I just use
address(this).balance to do it. 

The next major function I put together is the setAccounts() functions. This function lets me create a specific address for each account so the other functions will work.

To test the code I first set some accounts, and then I made a few deposits in both Wei and Ether to confirm it works. After that I then withdrew 5 ether and 10 ether from accounts 1 and 2, respectively.  In all these test cases I also check the account balance and lastToWithdraw amount and lastToWithdraw account where appropriate. Screenshots are in a separate folder for your reference.

## Technologies

I am using python version 3.7.10.  I go to the website https://remix.ethereum.org/ and run joint_savings.sol on the webpage and that's it.


---

## Installation Guide

I have python version 3.7.10 and git version 2.33.0.windows.2 installed on a laptop running windows 10 pro.

---


## Usage

go to the website https://remix.ethereum.org/ and run joint_savings.sol on the webpage and that's it. The user needs to compile
the code and then deploy it, and you should be able to test all the functions as needed.

---

## Contributors
Just me, Paul Lopez.


---

## License
No licenses required. Just install everything for free, pull from my repository, and enjoy!
