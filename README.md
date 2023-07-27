# AVALANCHE-MODULE4-PROJECT
# MyToken (Dengen - DGN)

MyToken is an Ethereum-based ERC20 token smart contract with additional features, designed to serve as an in-game currency for the game "Dengen."

## Contract Overview

The MyToken contract is based on the OpenZeppelin library and inherits from ERC20 and ERC20Burnable contracts, providing standard token functionality along with the ability to burn tokens. The contract also extends the Ownable contract, which ensures that only the owner of the contract can perform certain privileged operations.

## Functionalities

1. **Token Minting** (`mint` function):
   - The contract owner can mint new tokens and allocate them to specific addresses.
   - Only the contract owner can call the `mint` function.

2. **Token Redeeming** (`redeem` function):
   - Token holders can redeem their tokens for in-game items or any other specified purpose.
   - The `redeem` function allows token holders to burn their tokens, reducing their balance.
   - The specific redeeming logic should be implemented within the `redeem` function.

3. **Check Token Balance** (`checkBalance` function):
   - Token holders can check their token balance at any time by calling the `checkBalance` function.
   - The function takes an Ethereum address as input and returns the token balance for that address.

## Getting Started

To deploy your own instance of the MyToken contract:

1. Ensure you have the necessary development environment (e.g., Node.js, Truffle, Ganache, etc.) set up on your local machine.

2. Deploy the contract to the Ethereum network of your choice, preferably a test network first for testing and debugging.

3. After deployment, the contract owner can start minting new tokens using the `mint` function and allocate them to player addresses.

4. Players can interact with the contract to redeem tokens for in-game items by calling the `redeem` function. Make sure to implement the specific redeeming logic within the function.

5. Players can also check their token balance using the `checkBalance` function.

## Security Considerations

- Take security measures to protect the contract owner's private key.
- Test the contract thoroughly on test networks before deploying to the mainnet.
- Consider adding additional access control mechanisms if necessary for your specific use case.
- Be cautious about the redeeming logic to avoid unintended consequences and vulnerabilities.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
## Author
Jaya Singh
