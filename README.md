# AVALANCHE-MODULE4-PROJECT
Sure! Below is a simple README file for the ERC20 token smart contract named "Dengen" with the symbol "DGN" and the added in-game store functionality. This README provides a brief overview of the contract and its functionalities.

---

# Dengen Token (DGN) - In-Game Store README

The Dengen Token (DGN) is an ERC20-compliant token deployed on the Ethereum blockchain. It allows users to perform standard ERC20 token operations like transferring tokens, checking balances, and burning tokens. Additionally, the token contract includes an in-game store functionality, allowing players to redeem their tokens for items in the store.

## Contract Details

- Contract Name: `MyToken`
- Symbol: `DGN`
- Initial Supply: Deployer's address is credited with the total supply of tokens during deployment.

## Functionalities

1. Minting New Tokens
   - Function: `mint(address to, uint256 amount)`
   - Access: Only the contract owner can mint new tokens.
   - Purpose: The owner can create and distribute new tokens to players as rewards.

2. Adding Items to the In-Game Store
   - Function: `addItemToStore(string memory itemName, uint256 price, uint256 quantity)`
   - Access: Only the contract owner can add new items to the store.
   - Purpose: The owner can define new items in the store, specifying their token price and quantity.

3. Redeeming Tokens for Items in the In-Game Store
   - Function: `redeem(string memory itemName)`
   - Access: Players (anyone) can use this function.
   - Purpose: Players can redeem tokens from their balance for items available in the in-game store. Upon successful redemption, the tokens are transferred from the player to the owner's address (or designated account for the store).

4. Checking Token Balance
   - Function: `checkBalance(address player) public view returns (uint256)`
   - Access: Players (anyone) can check their token balance using this function.
   - Purpose: Players can verify their token balance at any time.

5. Checking In-Game Item Details
   - Function: `getInGameItemDetails(string memory itemName) public view returns (uint256 price, uint256 quantity)`
   - Access: Players (anyone) can check details of a specific in-game item using this function.
   - Purpose: This function provides information about the token price and available quantity of an item in the store.

## Usage

1. Deploying the Contract
   - Deploy the `MyToken` contract on the Ethereum blockchain using Remix or any other Ethereum development environment.

2. Minting Tokens
   - After deployment, the contract owner can mint new tokens using the `mint` function and distribute them to players.

3. Adding Items to the In-Game Store
   - The contract owner can add new items to the store by calling the `addItemToStore` function and providing the item's name, token price, and quantity.

4. Redeeming Tokens for Items
   - Players can redeem their tokens for items in the store by calling the `redeem` function with the item's name. The contract will handle the token transfer and update the store's item quantity.

5. Checking Token Balance and In-Game Item Details
   - Players can use the `checkBalance` function to verify their token balance and `getInGameItemDetails` function to check the details of a specific in-game item.

## Disclaimer

This contract is provided as an example and for educational purposes only. It is not audited and should not be used in production environments or with real funds without proper security reviews and testing.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
## Author
Jaya Singh
