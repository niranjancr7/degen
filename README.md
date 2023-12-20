# Token Contract 

## Overview

This is a Solidity smart contract written for the Ethereum blockchain. The contract, named `Token`, is an ERC-20 token with additional functionality for minting, transferring tokens, redeeming ornaments, and burning tokens.

## Features

1. **ERC-20 Compliance:** The contract follows the ERC-20 standard, making it compatible with various Ethereum wallets and decentralized applications.

2. **Minting Tokens:** The owner of the contract can mint new tokens and allocate them to specific accounts.

3. **Transferring Tokens:** Token holders can transfer tokens to other addresses, subject to availability.

4. **Redeeming Ornaments:** Users can redeem ornaments by spending a specific quantity of tokens. Each ornament has a defined token cost and quantity.

5. **Burning Tokens:** Token holders can burn their own tokens, reducing the total token supply.

## Contract Structure

- **Token Contract (`Token.sol`):** The main contract inheriting from ERC-20, Ownable, and ERC-20 Burnable.

- **Ornament Structure:** An internal struct, `Ornament`, stores information about each ornament, including its token cost and quantity.

- **Ornament Mapping:** The contract maintains a mapping of ornament names to their corresponding `Ornament` structures.

- **Event Logging:** The contract emits events (`LogMessage` and `OrnamentRedeemed`) to provide transparency and allow external applications to listen for specific activities.

## Deployment

The contract is deployed on the Ethereum blockchain with specified parameters for the initial supply of gold and silver coins.

## Usage

### Minting Tokens

The contract owner can mint new tokens using the `mint` function, specifying the recipient's address and the quantity of tokens to mint.

### Transferring Tokens

Token holders can transfer tokens to other addresses using the `transferTokens` function. Sufficient funds must be available in the sender's account.

### Redeeming Ornaments

Users can redeem ornaments by calling the `redeemOrnament` function, providing the ornament name and the quantity of tokens to spend. The contract checks the availability of tokens and the quantity of the specified ornament.

### Burning Tokens

Token holders can burn their own tokens using the `burnTokens` function, reducing the total token supply.


## Author

 niranjan D N

dnniranjan97@gmaol.com

## License

This contract is released under the MIT License. 
