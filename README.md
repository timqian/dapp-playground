## Folder structure
- `contracts/`: stores contracts
- `clients/`: stores clients interacting with contracts
- `migrations/`: stores scripts used to deploy contracts to eth blockchain

## Applications
1. SimpleStorage: Store and manipulating a value on blockchain [[`contract`](./contracts/01_SimpleStorage.sol) [`client`](./clients/01.js)]
2. PetAdoption: Pet Adoption app on blockchain[[`contract`](./contracts/02_PetAdoption.sol) [`client`](./clients/02.js)]
3. SimpleCoin: create a coin for yourself[[`contract`](./contracts/03_SimpleCoin.sol) [`client`](./clients/03.js)]
4. SimpleBank: create a central bank on blockchain [[`contract`](./contracts/04_SimpleBank.sol) [`client`](./clients/04.js)]
5. CrowdFund: A crowdfunding example (broadly similar to Kickstarter) [[`contract`](./contracts/05_CrowdFund.sol) [`client`](./clients/05.js)]
6. Content Management System [TODO]

## Deploy Contracts and test locally

1. Install and start [Ganache](https://truffleframework.com/ganache) (local, personal Ethereum blockchain)
1. Compile contracts
    ```bash
    npm run compile
    ```
1. Migrate contracts to local block chain
    ```bash
    npm run migrate
    ```
1. Interact with contracts
    ```bash
    npm run -- exec clients/01.js
    npm run -- exec clients/02.js
    ...
    ```

## Sample DAPPs on the main chain
- DAPP collection website: https://www.stateofthedapps.com/rankings
- oracle and prediction market: https://www.augur.net/
- Job Market Platform: https://ethlance.com/

## Good Readings
- Useful Ðapp Patterns: https://github.com/ethereum/wiki/wiki/Useful-%C3%90app-Patterns
- Web compiler `remix`: https://remix.ethereum.org/#version=builtin&optimize=false
- Official solidity doc: http://solidity.readthedocs.io/en/v0.4.24/introduction-to-smart-contracts.html
- Learn X in Y minutes solidity: https://learnxinyminutes.com/docs/solidity/
- web3 api: https://github.com/ethereum/wiki/wiki/JavaScript-API
- Awesome eth: https://github.com/btomashvili/awesome-ethereum
- About security: https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README-zh.md
- Other p2p solutions: https://github.com/kgryte/awesome-peer-to-peer
- solidity-baby-steps(might be a little outdated): https://github.com/fivedogit/solidity-baby-steps

## Ideas
### Make writing dapp as easy as possible
better than truffle
1. Write contract
2. Compile and deploy
3. Interact with contract

Is migrations script necessary?

compilers: web3; http://solidity.readthedocs.io/en/v0.4.24/installing-solidity.html#solcjs

### Decentrialized Github

## Questions and Answers
How to host content/app freely on decentrialized network? Currently facebook/github provide free content host and store, because they can get profit by ads etc to cover the cost. But on blockchain, hosting any content cost money, free users are a giant group, Is it possible to win them to blockchain?