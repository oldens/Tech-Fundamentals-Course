# Lesson 26: Practical Application: ERC-20 Tokens

## Topics
- ERC-20 standard
- How tokens are created on Ethereum (overview of tools, possibly demonstration in a test network)

## Notes
ERC-20 is a technical standard used for smart contracts on the Ethereum blockchain for implementing tokens. ERC-20 defines a common list of rules that all Ethereum tokens must follow, allowing developers to create interoperable tokens.

### ERC-20 Standard
The ERC-20 standard includes the following functions and events:

1. **Functions**:
   - `totalSupply()`: Returns the total supply of the token.
   - `balanceOf(address account)`: Returns the balance of the specified address.
   - `transfer(address recipient, uint256 amount)`: Transfers tokens from the caller's account to the recipient's account.
   - `approve(address spender, uint256 amount)`: Allows the spender to withdraw from the caller's account multiple times, up to the specified amount.
   - `transferFrom(address sender, address recipient, uint256 amount)`: Transfers tokens from the sender's account to the recipient's account using the allowance mechanism.
   - `allowance(address owner, address spender)`: Returns the remaining number of tokens that the spender is allowed to spend on behalf of the owner.

2. **Events**:
   - `Transfer(address indexed from, address indexed to, uint256 value)`: Emitted when tokens are transferred.
   - `Approval(address indexed owner, address indexed spender, uint256 value)`: Emitted when the allowance of a spender is set by a call to `approve`.

### How Tokens are Created on Ethereum
Creating ERC-20 tokens on Ethereum involves writing a smart contract that implements the ERC-20 standard. The following tools are commonly used for this purpose:

1. **Solidity**: A programming language for writing smart contracts on Ethereum.
2. **Remix**: An online IDE for developing, testing, and deploying smart contracts.
3. **MetaMask**: A browser extension that allows users to interact with the Ethereum blockchain.
4. **Ganache**: A personal blockchain for Ethereum development that allows you to deploy contracts, develop applications, and run tests.

#### Example of an ERC-20 Token Contract
Here is a simple example of an ERC-20 token contract written in Solidity:

```solidity
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract MyToken is ERC20 {
    constructor(uint256 initialSupply) ERC20("MyToken", "MTK") {
        _mint(msg.sender, initialSupply);
    }
}
```

In this example, the `MyToken` contract inherits from the `ERC20` contract provided by the OpenZeppelin library. The constructor initializes the token with a name ("MyToken") and a symbol ("MTK"), and mints the initial supply of tokens to the deployer's address.

### Demonstration in a Test Network
To demonstrate the creation and deployment of an ERC-20 token, you can use a test network such as Ropsten or Rinkeby. The steps involved are:

1. Write the smart contract in Solidity.
2. Compile the contract using Remix.
3. Deploy the contract to the test network using MetaMask.
4. Interact with the deployed contract to transfer tokens and check balances.

By understanding the ERC-20 standard and the process of creating tokens on Ethereum, you can develop your own tokens and explore the possibilities of decentralized finance (DeFi) and other blockchain applications.
