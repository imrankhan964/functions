# Token (Rocky)

## Overview

The Token (Rocky) smart contract is an Ethereum-based ERC-20 token with additional functionality for minting, burning, and transferring tokens. It is implemented in Solidity and utilizes the OpenZeppelin library for ERC-20 implementation and Ownable functionality.

## License

This smart contract is released under the MIT License. See the SPDX-License-Identifier at the top of the contract file for details.

## Smart Contract Details

### ERC-20 Standard

The Token (Rocky) contract is compliant with the ERC-20 standard, providing basic token functionalities such as transfers and balance management.

### Minting

The contract includes a minting function that allows the owner to create and allocate new tokens to a specified address. Minting can only be performed by the contract owner, providing a mechanism for controlled token issuance.

### Burning

Token holders can burn their own tokens using the burn function, reducing their token balance. This function helps manage the token supply by allowing users to destroy their tokens.

### Transferring

The transfer function inherits from the ERC-20 standard but includes additional checks. It ensures that the destination address is valid, the transfer amount is positive, and the sender has a sufficient balance. The function emits a custom event, `TokensTransferred`, upon a successful transfer.

### Events

The contract emits three events:

1. **TokensMinted:** Triggered when new tokens are minted and allocated to a specific address.

2. **TokensBurned:** Triggered when tokens are burned by a token holder.

3. **TokensTransferred:** Triggered when tokens are successfully transferred from one address to another.

## Constructor

The constructor initializes the token with the name "Rocky" and the symbol "RK." Additionally, it mints an initial supply of 500 tokens to the address specified during contract deployment.

## Deployment

The contract is deployed with the address of the creator, who becomes the initial owner of the contract. The owner has exclusive rights to mint new tokens.

## Usage

Developers can deploy and interact with the Token (Rocky) contract on the Ethereum blockchain. They can utilize the provided functions for minting, burning, and transferring tokens according to the ERC-20 standard.

## Imran khan

imrankhan924738@gmail.com
