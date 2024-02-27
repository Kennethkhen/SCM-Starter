# Assessment Smart Contract

## Overview

This is a Solidity smart contract named `Assessment` that implements basic functionalities for managing an account's balance, allowing deposits, withdrawals, and purchases of items. It includes event logging for key actions and custom error handling for specific scenarios.

## License

This project is licensed under the terms of the MIT license. See the [LICENSE](LICENSE) file for details.

## Prerequisites

- [Solidity](https://docs.soliditylang.org/en/latest/)

## Contract Details

- **Solidity Version:** ^0.8.9
- **Owner:** The owner of the contract, who has privileged access to deposit and withdraw funds.

## Functions

### `constructor(uint initBalance)`

- **Description:** Constructor to initialize the contract with an initial balance.
- **Parameters:**
  - `initBalance` (uint): The initial balance of the contract.

### `getBalance()`

- **Description:** Retrieves the current balance of the contract.
- **Returns:** `uint256`: The current balance.

### `deposit(uint256 _amount)`

- **Description:** Allows the owner to deposit additional funds into the contract.
- **Parameters:**
  - `_amount` (uint256): The amount of funds to deposit.

### `withdraw(uint256 _withdrawAmount)`

- **Description:** Allows the owner to withdraw funds from the contract.
- **Parameters:**
  - `_withdrawAmount` (uint256): The amount of funds to withdraw.

### `buy(string memory _item)`

- **Description:** Allows anyone to purchase items by specifying the item name.
- **Parameters:**
  - `_item` (string): The name of the item to purchase.

## Events

### `Deposit(uint256 amount)`

- **Description:** Emitted when funds are deposited into the contract.
- `amount` (uint256): The amount of funds deposited.

### `Withdraw(uint256 amount)`

- **Description:** Emitted when funds are withdrawn from the contract.
- `amount` (uint256): The amount of funds withdrawn.

### `ItemBought(string item, uint256 price)`

- **Description:** Emitted when an item is successfully purchased.
- `item` (string): The name of the purchased item.
- `price` (uint256): The price of the purchased item.

## Custom Error

### `InsufficientBalance(uint256 balance, uint256 withdrawAmount)`

- **Description:** Custom error thrown when attempting to withdraw more funds than the contract balance.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Support

For support, contact [Your Email Address].

## Disclaimer

This code is provided as-is, without any warranty or support. Use at your own risk.

