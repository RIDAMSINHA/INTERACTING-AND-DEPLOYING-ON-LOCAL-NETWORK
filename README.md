# RIDAM Token (RUK) README

## Introduction

Welcome to the RIDAM Token (RUK) repository! This repository contains the Solidity smart contract code for the RUK token, an ERC-20 compatible token designed for various purposes. RUK tokens can be used for transactions, rewards, and other activities within an ecosystem.

This README file provides an overview of the RUK token contract and includes instructions on how to deploy the contract to the local Hardhat test network using Remix Connect Localhost and how to interact with it using Remix with Hardhat provider.

## Contract Details

The `Token.sol` file contains the source code for the RUK token contract. Here are the key details of the contract:

- Token Name: RIDAM Token
- Token Symbol: RUK
- Decimals: 18
- Total Supply: 0 (initially)

The contract includes standard ERC-20 functions such as `balanceOf` and `transfer`. It also includes functionalities for minting and burning tokens, accessible only by the contract owner.

The contract owner has special privileges and is the only address allowed to mint new tokens. Other addresses can interact with the contract by transferring tokens and burning their own tokens.

## Deployment on Local Hardhat Test Network using Remix Connect Localhost

To deploy the RUK token contract to the local Hardhat test network using Remix Connect Localhost, follow these steps:

1. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

2. Create a new file named `Token.sol` and copy the contents of the `Token.sol` file from this repository into it.

3. Select the Solidity compiler version `0.8.0` or a compatible version.

4. Compile the contract by clicking the "Compile" button.

5. Switch to the "Deploy & Run Transactions" tab.

6. In the "Environment" dropdown, select "Web3 Provider".

7. In a separate terminal, navigate to your project directory and run the local Hardhat network using the command: `npx hardhat node`.

8. Copy the URL of the local Hardhat network provided in the terminal (e.g., `http://127.0.0.1:8545`).

9. Paste the copied URL into the "Web3 Provider Endpoint" input field in Remix.

10. Click the "Deploy" button next to the `Token` contract.

11. Confirm the deployment transaction in Remix.

12. Wait for the deployment transaction to be confirmed on the local Hardhat network.

13. Once the contract is deployed, you will see the contract address in the Remix console. Make note of this address for future interactions.

## Interacting with the Contract using Remix with Hardhat Provider

After deploying the RUK token contract to the local Hardhat test network, you can interact with the contract using Remix with Hardhat provider. Here are the steps to get started:

1. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

2. In the "File Explorer" section, locate the `Token.sol` file and open it.

3. In the "Deployed Contracts" section, click on the contract named `Token`.

4. In the "At Address" input field, enter the contract address obtained during deployment.

5. Click the "At Address" button to load the contract instance.

6. You can now interact with the RUK token contract through the provided functions.

   - Use the `balanceOf` function to check the token balance of a specific address.
   - Use the `transfer` function to send RUK tokens from your address to another address.
   - Use the `mint` function (accessible only to the contract owner) to mint

 new RUK tokens.
   - Use the `burn` function to burn a specific amount of your RUK tokens.

7. Set the required parameters for each function and click the corresponding button to execute the transaction.

8. Confirm the transaction details and sign the transaction in Remix.

9. Wait for the transaction to be confirmed on the local Hardhat network.

10. You can view the transaction status and emitted events in the Remix console.

## Authors

RIDAM ADITYA SINHA

https://www.linkedin.com/in/ridam-sinha-188133210/

ridamsinha20@gmail.com

## License

The RIDAM Token (RUK) contract is licensed under the MIT License. See the [`LICENSE`](LICENSE) file for more information.

## Disclaimer

Please note that this contract and the associated README file are provided for informational purposes only. Deploying and interacting with smart contracts involves risks, and it is your responsibility to review and understand the code before proceeding. Make sure to exercise caution and perform appropriate testing before deploying any smart contract on a live network.
