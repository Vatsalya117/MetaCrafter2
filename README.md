# Solidity Smart Contract for MyToken

This Solidity smart contract is designed for managing non-fungible tokens (NFTs) on the Ethereum blockchain. It includes functionalities for minting new NFTs, burning existing NFTs, and managing the token supply.

## Requirements

1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
2. Your contract will have a mapping of addresses to balances (address => uint)
3. You will have a mint function that takes two parameters: an address and a value. The function then increases the total supply by that number and increases the balance of the “sender” address by that amount
4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. It will take an address and value just like the mint functions. It will then deduct the value from the total supply and from the balance of the “sender”.
5. Lastly, your burn function should have conditionals to make sure the balance of the "sender" is greater than or equal to the amount that is supposed to be burned.

## Contract Details

### Public Variables

- `tokenName`: The name of the token (e.g., "ALPHA").
- `tokenAbbreviation`: The abbreviation of the token (e.g., "Beta").
- `totalSupply`: The total supply of the token.


### Getting Started

#### SPDX-License-Identifier:

This line indicates the license under which the code is released. In this case, it's using the MIT License, which is a permissive open-source license.

#### Solidity Version:

pragma solidity ^0.8.0; specifies the version of the Solidity compiler that should be used to compile the contract. In this case, it requires version 0.8.0 or higher.

#### Contract MyToken:

tokenName, tokenAbbreviation, and totalSupply are public variables storing the name, abbreviation, and total supply of the token.

balances is a mapping that associates addresses with their token balances.

mint function takes two parameters (_address and _value) and increases the total supply by _value, adding _value tokens to the balance of the specified _address.

burn function takes two parameters (_address and _value) and checks if the balance of _address is sufficient to burn _value tokens. If so, it decreases the total supply by _value and deducts _value tokens from the balance of _address.

### Help
If you encounter any issues or have questions, please refer to the documentation or contact the contributors:

### Authors

Vatsalya Mishra

https://github.com/Vatsalya117
