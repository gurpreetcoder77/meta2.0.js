DESCRIPTION

In this project of token creation first i have created a contract which will store the details of my token such as token name, token abbr. and total supply. I had made these variables as public.

Second step is to create a mapping variable to track how many tokens each address holds. The keys of the mapping are Ethereum addresses. The values are unsigned integers representing the token balance associated with each address.

Third step is to create a mint function that allows new tokens to be added to the assigned adderess. Parameters are _value and _address. Increases the totalSupply by the _value and Increases the balance of the _to address by the _value. For simplicity this function has been made public.

Forth step is to create another function named burn function. Functionality of this function is to destroy tokens by a specific value from the given address which is opposite to that of mint function. functions Checks if the balance of the _from address is greater than or equal to the _value to be burned. If sufficient balance exists, it decreases the totalSupply by _value and decreases the balance of the _from address by _value. The burn function includes a crucial check to prevent errors: Before burning tokens, it verifies that the address initiating the burn (_from) has enough tokens to cover the amount being burned. This prevents accidental over-burning and helps maintain the integrity of the token's supply.


# ETH-PROOF Beginner EVM Course - Metacraft

This is a simple Smart Contract program written in Solidity. The contract allows for minting and burning of tokens, while keeping track of balances associated with different addresses. It includes the following features:

- Public variables to store token details such as name, abbreviation, and total supply.
- A mapping to track balances of different addresses.
- Functions to mint and burn tokens, updating the total supply and balances accordingly.

## Getting Started

To run this code, follow these steps:

1. Go to [Remix Ethereum IDE](https://remix.ethereum.org).
2. Import code.sol.
3. Run and debug the code.

## Author

Created by: gurpreet yadav

## License

This project is licensed under the MIT License.
