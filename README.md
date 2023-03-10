# ๐ Scaffold-Balancer

> everything you need to build on Balancer! ๐

๐งช Quickly experiment with custom AMMs using a frontend that allows you to interact with your custom pool contract(s).

๐งช Fork mainnet ethereum and test your custom pools within the context of all available liquidity.

๐ Build and test your Smart Order Router (SOR) extension, getting you one step closer to being integrated into the Balancer ecosystem.

## Features

This project is a fork of scaffold-eth-typescript with a focus on providing [Balancer]:

- A react frontend running with `nextjs`.
- Solidity toolkit of `hardhat` or `foundry`

# ๐โโ๏ธ Quick Start

Prerequisites: [Node (v16)](https://nodejs.org/en/download/) plus [Yarn (v1.x)](https://classic.yarnpkg.com/en/docs/install/) and [Git](https://git-scm.com/downloads)

> 1๏ธโฃ clone/fork ๐ scaffold-balancer:

```bash
git clone https://github.com/beethovenxfi/scaffold-balancer.git
```

> 2๏ธโฃ Install all necessary dependencies

```bash
yarn install
```

> 3๏ธโฃ start your ๐ทโ Hardhat fork of mainnet ethereum:

```bash
yarn fork
```

> 4๏ธโฃ in a second terminal window, start your ๐ฑ frontend:

```bash
yarn dev
```

> 4๏ธโฃ in a third terminal window, ๐ฐ deploy your contract:

โ ๏ธ By default any existing contract deployments are triggerred when you start your fork of mainnet `yarn fork`. This stay may not be required.

```bash
yarn deploy
```

๐ Edit your smart contract `YourCustomPool.sol` in `packages/solidity-ts/contracts`

๐ผ Edit your contract deployment scripts in `packages/solidity-ts/deploy`

๐ Edit your frontend in `packages/nextjs-app-ts/src`

๐ป Open http://localhost:3000 to see the app

## Configuration

Scaffold uses `scaffold.config.json` as a configuration file located in `/packages/common/src/scaffold.config.json`. You can create the config file by running the command `yarn create-config`.
