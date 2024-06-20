MyToken Smart Contract
Overview
MyToken is a basic ERC-20-like token implemented in Solidity. This contract allows for the creation (mint) and destruction (burn) of tokens. It includes public variables for the token's name, symbol, and total supply, and it uses a mapping to keep track of balances associated with each address.

Features
Token Name: Token
Token Symbol: MTK
Total Supply: Dynamically updated with minting and burning actions
Minting: Allows the creation of new tokens and assigns them to a specified address
Burning: Allows the destruction of tokens from a specified address, reducing the total supply
Getting Started
Prerequisites
Solidity ^0.8.18
A development environment such as Remix or Truffle
Installation
Clone the repository:

sh
git clone https://github.com/yourusername/MyToken.git
cd MyToken
Open the contract in your preferred development environment:

For Remix, you can directly copy and paste the code.
For Truffle, place the contract file in the contracts directory.
Usage
Deploy the contract:

In Remix, compile the contract and deploy it using the provided deploy button.
In Truffle, run truffle migrate to deploy the contract to your configured network.
Mint Tokens:
Call the mint function with the recipient's address and the amount of tokens to be created.

solidity
Copy code
function mint(address _to, uint256 _value) public
Burn Tokens:
Call the burn function with the owner's address and the amount of tokens to be destroyed.

solidity
function burn(address _from, uint256 _value) public
Example
To mint 100 tokens to address 0x123...456:

solidity
Copy code
myToken.mint("0x123...456", 100);
To burn 50 tokens from address 0x123...456:

solidity
myToken.burn("0x123...456", 50);
Contributing
Contributions are welcome! Please feel free to submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
