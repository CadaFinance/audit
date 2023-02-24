# Cada-contract

The smart contracts behind cada.finance

The contracts are compiled with Hardhat, and tested using Waffle and TypeScript.
Installation

$ npm i

Usage
Build

$ npm run build

Test

$ npm test

Coverage

$ npm run coverage

Deploying contracts to localhost Hardhat EVM

$ npm run start

You can connect to this RPC server via http://localhost:8545 with chain ID of 31337
Deploying contracts to local fork of Mainnet

In order to successfully fork the mainnet, ALCHEMY_API must be set to a valid URL in the .env file.

ALCHEMY_API="https://eth-mainnet.alchemyapi.io/v2/XXXXXXXXXXXX"

$ npm run fork

You can connect to this RPC server via http://localhost:8545 with chain ID of 1.
Deploying contracts to Ropsten

In order to successfully deploy to Ropsten, ALCHEMY_API_ROPSTEN must be set to a valid URL in the .env file. MNEMONIC_TEST_ACCOUNT must be set and the accounts must have some rEth for successful deployments.

ALCHEMY_API="https://eth-ropsten.alchemyapi.io/v2/XXXXXXXXXXXX"
MNEMONIC_TEST_ACCOUNT="seed phrase"

Generating GitBook docs

$ npx solidity-docgen --templates=templates

The output in the docs folder should be copied to the appropriate folder in the sirius-docs repo.
Running Slither

Slither is a Solidity static analysis framework. To run it locally:

$ pip3 install slither-analyzer
$ slither .

Slither is configured to run as a GitHub Action and error on any high findings.
