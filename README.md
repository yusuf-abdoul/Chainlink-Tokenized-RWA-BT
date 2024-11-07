# Tokenized Real-World Assets (RWA) Bootcamp Project

## Overview
This project was developed during the **Tokenized RWA Bootcamp** organized by **Chainlink**. The goal was to tokenize real estate assets using the **Zillow API** and deploy smart contracts on the **Avalanche Fuji Testnet**. The project features tokenization of real estate, **RWA Lending & Borrowing**, and **English Auction** capabilities. The **ERC-1155 token standard** was used to represent real estate assets, combining fungibility (ERC-20) and uniqueness (ERC-721).

## Technologies Used
- **Solidity** for smart contract development
- **Chainlink Automation & Chainlink Functions** to fetch real-time pricing data from the Zillow API
- **Avalanche Fuji Testnet** for smart contract deployment
- **ERC-1155 token standard** for asset tokenization
- **Chainlink VRF** (Verifiable Random Function) for secure randomness in auctions

## Smart Contracts

The following smart contracts were developed and deployed on the **Avalanche Fuji Testnet**:

1. **RealEstateToken.sol**  
   - Tokenizes real estate assets as **ERC-1155** tokens, allowing fractional ownership and trade of real estate properties.

2. **Issuer.sol**  
   - Manages the issuance of **RealEstateToken** and facilitates minting of new tokens that represent real estate properties.

3. **RWALending.sol**  
   - Implements **Lending & Borrowing** mechanisms for tokenized real estate, enabling users to lend or borrow assets based on tokenized property values.

4. **EnglishAuction.sol**  
   - Enables **English Auction** for tokenized real estate assets, allowing users to bid on fractional ownership of real estate properties.

## Project Details

### Tokenization
We used the **ERC-1155** token standard to represent real estate assets. This standard allowed us to create tokens that:
- Maintain the **fungibility** of ERC-20 tokens for real estate values.
- Retain the **unique attributes** of each asset like ERC-721 tokens, representing individual properties.

### Chainlink Integration
Through **Chainlink Automation** and **Chainlink Functions**, we:
- Automatically fetch real-time pricing data from the **Zillow API** to update the value of tokenized properties.
- Integrate this data into the smart contracts to ensure the real estate tokens reflect accurate market prices.

### RWA Lending & Borrowing
The **RWALending.sol** contract facilitates **Lending & Borrowing**:
- Users can lend their tokenized real estate assets and earn interest.
- Users can borrow against their tokenized real estate holdings, creating a decentralized finance (DeFi) system for tokenized properties.

### English Auction
The **EnglishAuction.sol** contract allows tokenized real estate assets to be auctioned:
- Users can bid on fractionalized ownership of properties, with the highest bidder receiving the asset.

### Issuance (Future Scope)
Currently, the **Issuance** step—deploying the smart contracts, minting tokens, and making them available for usage—was not covered in this scope of the project. We have focused on developing and testing the smart contracts, including tokenization, lending, borrowing, and auctions. However, we plan to implement **Issuance** in the future, potentially as part of a **real estate marketplace**, **Nestblock**. This will allow users to mint and trade tokenized real estate assets on the platform.

## How it Works

1. **Real Estate Data:** Chainlink Automation fetches real-time data from the **Zillow API** and updates real estate asset prices.
2. **Token Minting & Issuance:** While the minting of tokens is demonstrated in this project, the **Issuance** process, involving the deployment of tokens for trading and usage, is planned for future implementation.
3. **Lending & Borrowing:** Users can use the **RWALending.sol** contract to lend or borrow tokenized real estate assets.
4. **Auction:** The **EnglishAuction.sol** contract facilitates bidding on fractionalized real estate ownership through an English Auction process.

### Minting Process
For demonstration purposes, a mock version of real estate properties was minted directly to the deployer's wallet (my wallet). This was done to test the basic functionality of tokenizing assets but is not the final minting process for a real estate marketplace.

## Conclusion
This project explores the potential of tokenizing real-world assets (RWAs) and integrating them with decentralized finance (DeFi) functionalities such as **Lending & Borrowing** and **English Auctions**. By leveraging **Chainlink**'s decentralized oracle network, we ensured real-time pricing updates and randomness in the auction process.

---

## To Do (Future Enhancements)
- Implement **Issuance** of tokenized real estate assets as part of a marketplace (Nestblock).
- Deploy the solution on the **Avalanche C-Chain** mainnet for live transactions.
- Expand **RWALending.sol** with more complex lending mechanisms.

---

### License
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

