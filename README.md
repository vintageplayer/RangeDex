# Uniswap V3 Built From Scratch

This repo implements the Uniswap V3's ranged based liquidity provision and swapping with better capital efficiency with slippage control in a given price range.

It also implements the multi-pool swap allowing swapping of token pairs even if an explicit pool doesn't exist.

![Front-end application screenshot](/screenshot.png)

## How to Run
1. Ensure you have [Foundry](https://github.com/foundry-rs/foundry) installed.
1. Run Anvil:
    ```shell
    $ anvil
    ```
1. Set environment variables and deploy contracts:
    ```shell
    $ source .envrc
    $ make deploy
    ```
1. Install the Frontend Dependencies:
    ```shell
    $ cd ui && yarn install
    ```
1. Start the UI:
    ```shell
    $ yarn start
    ```
1. In Metamask, import this private key and add network `localhost:8545` with chain ID 31337:
    ```
    0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80
    ```
1. Enjoy!