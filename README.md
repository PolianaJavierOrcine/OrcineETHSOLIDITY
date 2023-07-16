# ETHEREUM
Ethereum operates a computer called the Ethereum Virtual Machine (EVM), which is effectively a single decentralised system. Any interactions must be confirmed so that everyone can update their copy because each node has a copy of that computer.The Ethereum blockchain stores network interactions as "transactions" that are contained within blocks. As a digital ledger or transaction history, miners validate these blocks before committing them to the network.

## Description
decentralized blockchain platform that establishes a peer-to-peer network that securely executes and verifies application code, called smart contracts.

## Getting Started

### Executing program
Using Remix, an online Solidity IDE, you may run this programm. To get started, go to the Remix website at https://remix.ethereum.org/.Once on the Remix website, create a new file by clicking on the "+" symbol in the left-hand sidebar.

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

## Authors
Poliana Javier Orcine

