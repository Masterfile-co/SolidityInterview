# SolidityInterview

This set of questions shouldn't take more than 30-45 minutes to finish. [Hardhat](https://hardhat.org/getting-started/) framework is used for this repo. To test contracts run `npx hardhat test`. You can use ethers.js or web3.js to write tests. If any of the instructions are unclear, just leave a comment with your interpretation of the problem and continue to solve from there. Once complete, please create a zip folder containing all files execpt for node_modules and email to garrett@masterfile.co with your Solidity Interview - Your Name in the subject line. These problems are not meant to be challenging, but mostly to show off your thought process. 

## Problem #1 

The goal is to create an ERC-721 contract that allows any user to mint a new token if they deposit at least 1 ether. Add as much commenting as needed to communicate the intended functionality. [Open Zepplin](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC721/ERC721.sol) is a good starting point for this problem.

Success Criteria:

- Contract must be fully ERC-721 compliant
- Add an extra `mint()` function that requires a deposit of 1 ether

## Problem #2 

Write tests to ensure proper functionality of contract

Success Tests:
- User can mint token if they send 1 eth
- calling `balanceOf()` shows that User has 1 minted token
- `Transfer` event is properly emited 

Failure Tests:
- User cannot mint token if they send less than 1eth
