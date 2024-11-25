# Simple Counter Token (SCT)

The **Simple Counter Token (SCT)** is a custom ERC20 token designed to work on the Avalanche Fuji Testnet. It supports token minting, transferring, and burning while incorporating an in-game store feature that allows users to redeem tokens for items. The contract also includes a counter feature to track incremental changes, which can be used in games or other applications.

## Features

- **Token Management**
  - Mint new tokens (Owner-only).
  - Transfer tokens between users.
  - Burn tokens from the user's balance.

- **In-Game Store**
  - Redeem tokens for in-game items.
  - View a list of available items in the store.
  - Track items redeemed by the user.

- **Counter Functionality**
  - Increment and decrement the counter.
  - Retrieve the current counter value.

- **Zero Decimals**
  - Tokens are non-fractional, ensuring only whole numbers are used.

## Deployment

The smart contract is deployed on the Avalanche Fuji Testnet, and all transactions can be verified on the [Snowtrace Explorer](https://testnet.snowtrace.io/).

### Contract Address
```
0xD2075459E4748264aA714D672f7d5268C49A91af
```

## How to Use

### 1. Mint Tokens
Mint tokens to an address (owner-only function):

This transaction is visible on **Snowtrace**.

### 2. View Available Items
Retrieve the list of items available for redemption:


### 3. Redeem Items
Redeem tokens for an item using the `redeemItem` function:

Transaction details, including the token burn, are visible on **Snowtrace**.

### 4. Transfer Tokens
Transfer tokens to another user:

The transfer can be verified on **Snowtrace**.

### 5. Use the Counter
Increment or decrement the counter:


### 6. Burn Tokens
Burn tokens from your balance:

This transaction will also appear on **Snowtrace**.

## Example Store Items
The contract includes predefined items in the in-game store:
- Item A: 100 tokens
- Item B: 200 tokens

Additional items can be added by the contract owner using the `addItem` function.

## Technical Details
- **Programming Language:** Solidity
- **Compiler Version:** 0.8.18
- **Frameworks Used:** OpenZeppelin (ERC20 and Ownable modules)

## Notes
- The token contract overrides the `decimals()` function to enforce zero decimals.
- Administrative functions (e.g., minting tokens, adding items) are restricted to the contract owner.

## Transaction Verification
All transactions, including minting, transfers, item redemptions, and token burns, can be viewed transparently on the Avalanche Fuji Testnet using **Snowtrace**. This ensures trust and accountability.

## License
This project is licensed under the MIT License.

