**MyToken**

MyToken is an ERC-20 compliant token contract written in Solidity.

**Features**
- ERC-20 compliant
- Allows for transfers, approvals, and allowances
- Includes functions to increase and decrease allowances

**Usage**
To use this contract, deploy it to an Ethereum network using a tool like Remix or Truffle. Once deployed, you can interact with the contract using its public functions.

**Constructor**
The constructor takes four arguments:
- string memory _name: The name of the token.
- string memory _symbol: The symbol of the token.
- uint8 _decimals: The number of decimal places for the token.
- uint256 initialSupply: The initial supply of tokens.

**Public Functions**
The contract includes several public functions that allow you to interact with the token:
1. `totalSupply()`: Returns the total supply of tokens.
2. `balanceOf(address account)`: Returns the balance of the specified account.
3. `transfer(address recipient, uint256 amount)`: Transfers the specified amount of tokens from the sender’s account to the recipient’s account.
4. `allowance(address owner, address spender)`: Returns the remaining number of tokens that the spender is allowed to spend from the owner’s account.
5. `approve(address spender, uint256 amount)`: Allows the spender to spend the specified amount of tokens from the sender’s account.
6. `transferFrom(address sender, address recipient, uint256 amount)`: Transfers the specified amount of tokens from the sender’s account to the recipient’s account, using an allowance.
7. `increaseAllowance(address spender, uint256 addedValue)`: Increases the allowance of the spender by the specified value.
8. `decreaseAllowance(address spender, uint256 subtractedValue)`: Decreases the allowance of the spender by the specified value.

**Events**
The contract emits two events:
- `Transfer(address indexed from, address indexed to, uint256 value)`: Emitted when tokens are transferred.
- `Approval(address indexed owner, address indexed spender, uint256 value)`: Emitted when an allowance is approved.

**License**
This project is licensed under the MIT License. See LICENSE for more information.