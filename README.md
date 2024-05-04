# ERC20 Assessment
In this third module, we're talking about ERC20 and OpenZepplin which are the two important components within the entirety of the module itself. Functionality and How to know and get them to work only with a few codes behind. These are the steps on how it'll be possible to run your token using Remix Ethereum and a little help with other sites as well.

# Description
This program is a simple contract written in Remix Ethereum, a programming language used for developing smart contracts using OpenZepplin, a give-and-take website that gives you free Codes for Tokens and in doing so takes a lot of people to their cause. These are a few codes in that can work perfectly in your favor as OpenZepplin gives you a GitHub that automatically gives you your initial code without even typing it. Just give a little more minting and coding and voila! done very easily.

## Getting Started
First off are the applications and GitHub;
Open the website OpenZepplin and find a GitHub of your choice, it's pretty easy and only open it within your tab for further use. 
Next is remix Ethereum, just open that badboy, and voila! you're good to go!

### Coding
First off is this command, go to remix Ethereum and create a file called "token.sol" (sol is important as it is the .sol that differs from other code) put these commands first
```
// SPDX-License-Identifier: UNLICENSEDS
//SPDX-Lisence-Identifier: MIT
pragma solidity ^0.8.20;
import "github of openzepplin";

```
Pragma Solidity is the one you need to see, you can change the version if you go to the "Solidity compiler" to check if you're up to date or if you want to change the compiler. 
importing the GitHub is the first and foremost of what you need to do, then run it so it'll read  the GitHub itself.

```
contract GrandielToken is ERC20("Grandiels Token", "GT"){

    function mintFifty() public {
        _mint(msg.sender, 50 * 10**18);
    }
    
}
```
Contract (the name of your token) is ERC20. ERC20 is the important one in this code here as it is to call the contract inside the OpenZepplin

Function mintfifty is the one you also need to do to give it functionality.
(msg.sender) < this is before the calculation of 50 * 10**18 
the 50 * 10**18 is the equation I wanted to do as tokens do not like decimals in their tokens.

## Running the code
Once you are all done there you need to do a ctrl + s to see if you have discrepancies in your code, if you don't have then voila! go to deploy and run, copy your address, and deploy your code. If you deployed it you need to scroll down and go to "deployed contracts" and youll see the blue "balanceof" there you'll paste the address you copied and run too see if theres any tokens you own(which is zero at the moment). once youre finished, go to mintfifty and press it, go to balanceof again to run and voila! you have at least 500000000 tokens!

# Authors
Jay-Ann S. Rafanan/ 3.1BIST/ NTC/ Sakiwaree

# License
This project is licensed under the MIT License - see the LICENSE.md file for details
