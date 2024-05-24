# Solidity-project
@@ -1,10 +1,11 @@
MyToken Smart Contract
MYTOKEN SMART CONTRACT

DESCRIPTION
DESCRIPTION:

The MyToken contract is a simple implementation of a token system in Solidity, designed to handle basic minting and burning of tokens. The contract defines public variables for the token's name, abbreviation, and total supply, making this information easily accessible. It uses a mapping to keep track of the balance of tokens held by each address, ensuring precise and transparent management of individual holdings. The mint function allows for the creation of new tokens, incrementing the total supply and updating the balance of a specified address. Conversely, the burn function permits the destruction of tokens, provided the address has sufficient balance, thereby decreasing both the total supply and the address's token holdings. This straightforward structure provides essential functionality for managing a token economy on the Ethereum blockchain.

Requirements
REQUIRMENTS:

1.Public Variables: The contract includes public variables to store details about the token:

Token Name (tokenName)
@@ -17,7 +18,7 @@ Total Supply (totalSupply)

4.Burn Function: A function to decrease the total supply of tokens and deduct them from a specified address, with a check to ensure the address has enough tokens to burn.

Contract Code:
CONTRACT CODE:

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;
@@ -46,7 +47,8 @@ contract MyToken {
    }
}

Functions:
FUNCTIONS:

Mint Function
Tokens can be created anew through the mint function. Upon calling, it adds the specified _value to the balance of the specified _address and raises the totalSupply by that amount.

@@ -63,11 +65,11 @@ function burn(address _address, uint _value) public
_address: The address from which the tokens will be burned.
_value: The number of tokens to burn.

Usage:
USAGE:
Deploy the MyToken contract to the Ethereum blockchain using your preferred method Remix.

After deployment, you can interact with the contract to mint and burn tokens, as well as check the balances and total supply.


License
LICENSE:
This contract is licensed under the Metacrafters License.
