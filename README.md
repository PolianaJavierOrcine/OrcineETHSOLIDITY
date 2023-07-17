## Solidity

Smart contracts can be created using Solidity, a high-level, contract-oriented programming language. Solidity is an object-oriented programming language developed expressly by the Ethereum Network team for developing and designing smart contracts on Blockchain systems. Solidity was intended to interact with the Ethereum Virtual Machine (EVM) and is significantly influenced by C++, Python, and JavaScript.

## Description
Solidity is an object-oriented programming language developed exclusively by the Ethereum Network team for developing and implementing smart contracts on Blockchain platforms. It is used to establish smart contracts that implement business logic and produce a chain of transaction records in the blockchain system.using is used for including a library within a contract in solidity. Check this following example: pragma solidity ^0.4.15;library SomeLibrary { function add(uint self, uint b) returns (uint) { return self+b; }
## Getting Started

### Executing program

### Installing
We recommend Remix for small contracts and for quickly learning Solidity.
Access Remix online, you do not need to install anything. If you want to use it without connection to the Internet, go to https://github.com/ethereum/remix-live/tree/gh-pages and download the .zip file as explained on that page. Remix is also a convenient option for testing nightly builds without installing multiple Solidity versions.
Further options on this page detail installing commandline Solidity compiler software on your computer. Choose a commandline compiler if you are working on a larger contract or if you require more compilation options.

### Executing program
Step 1:Copy the given code in Remix IDE Code Section.

Step 2:Under Compile Tab, click Start to Compile button.

Step 3:Under Run Tab, click Deploy button.

Step 5:Under Run Tab, Select SolidityTest at 0x... in drop-down.

Step 6:Click getResult Button to display the result.

ORCINE_SOLIDITY.sol

By selecting the "Deploy & Run Transactions" tab in the left-hand sidebar after the code has been compiled, you can launch the contract. From the drop-down menu, choose the "HelloWorld" contract, and then press the "Deploy" button.

### Help
In essence, Solidity's error handling maintains atomicity as a trait. All state changes (i.e., adjustments made to variables, balances, etc.) are undone all the way up the chain of contract calls when a smart contract call concludes with an error.

## Authors
Poliana Javier Orcine

@PolianaJavierOrcine



