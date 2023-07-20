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


// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

/*
       REQUIREMENTS
    1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
    2. Your contract will have a mapping of addresses to balances (address => uint)
    3. You will have a mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly, your burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.
*/

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

By selecting the "Deploy & Run Transactions" tab in the left-hand sidebar after the code has been compiled, you can launch the contract. From the drop-down menu, choose the "HelloWorld" contract, and then press the "Deploy" button.

### Help

In essence, Solidity's error handling maintains atomicity as a trait. All state changes (i.e., adjustments made to variables, balances, etc.) are undone all the way up the chain of contract calls when a smart contract call concludes with an error.

## Authors

Poliana Javier Orcine

Gmail-8210778@ntc.edu.ph

@PolianaJavierOrcine



