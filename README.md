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

contract MyToken {

// public variables here

       string public tokenName="SOLIDITY";
       string public tokenAbbrv="SLIDTY";
       uint public totalSupply=0;

// mapping variable here
    
    mapping(address => uint) public balances;

// Mint function
       
        function mint(address recipient, uint value) public {
        totalSupply += value;
        balances[recipient] += value;
    }
    
// burn function
       
       function burn(address add, uint val) public {
        if (balances[add] >= val){
        totalSupply -= val;
        balances[add] -= val; 
        }
    } 
    }

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile Assessment.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "Assessment" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can copy to the clipboard and paste it on burn, mint and balances in the deployed contracts. Put any amount of token you want in value, so that you can mint it. Check the amount of token you minted in totalSupply and balances, Once you confirm it you can now burn it by puttting how much the amount of tokens you want to burn because it will be subtracted to the tokens that minted then click on the "burn" function. Finally, click on the "transact" button to execute the function and you will see how much tokens you have left.


### Help

In essence, Solidity's error handling maintains atomicity as a trait. All state changes (i.e., adjustments made to variables, balances, etc.) are undone all the way up the chain of contract calls when a smart contract call concludes with an error.

## Authors

Poliana Javier Orcine

Gmail-8210778@ntc.edu.ph

@PolianaJavierOrcine



