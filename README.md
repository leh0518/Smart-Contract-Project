# MyToken Contract

This contract implements a basic ERC-20 token called "TOKEN" with the abbreviation "TKN". It allows for token minting, burning, and provides an example function.

## Contract Details

- **Solidity Version:** 0.8.18
- **License:** MIT

## Usage

### `mint(address _address, uint _value)`

Mints new tokens and assigns them to a specified address. The function takes two parameters:

- `_address` (address): The address to which the tokens will be assigned.
- `_value` (uint): The amount of tokens to mint.

The function checks that the provided address is not the zero address and then increases the total token supply and updates the balance of the specified address accordingly.

### `burn(address _address, uint _value)`

Burns existing tokens from a specified address. The function takes two parameters:

- `_address` (address): The address from which the tokens will be burned.
- `_value` (uint): The amount of tokens to burn.

The function checks that the provided address is not the zero address and that the address has a sufficient balance to burn the specified amount of tokens. It then decreases the total token supply and updates the balance of the specified address accordingly.

### `exampleFunction(uint _value)`

An example function demonstrating the usage of `revert` and `assert` statements. The function takes one parameter:

- `_value` (uint): The value to be evaluated.

The function uses an `assert` statement to check that the value is greater than zero. If the condition is not met, an exception is thrown. Additionally, if the value is less than 10, a `revert` statement is triggered, reverting any changes made before the call to `exampleFunction`.

## License

This code is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
