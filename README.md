# Alium Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain and Alium ecosystem.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repo:

1. **[Blocks](https://thegraph.com/explorer/subgraph/alium-official/blocks)**: Tracks all blocks on Binance Smart Chain.

2. **[Pairs](https://thegraph.com/explorer/subgraph/alium-official/pairs)**: Tracks all Alium Pairs and Tokens.

3. **[Exchange](https://thegraph.com/explorer/subgraph/alium-official/exchange)**: Tracks all Alium Exchange data with price, volume, liquidity, ...

4. **[Profile](https://thegraph.com/explorer/subgraph/alium-official/profile)**: Tracks all Alium Profile with teams, users, points and campaign.

5. **[Timelock](https://thegraph.com/explorer/subgraph/alium-official/timelock)**: Tracks all timelock transactions queued, executed, and cancelled.

6. **[SmartChef](https://thegraph.com/explorer/subgraph/alium-official/smartchef)**: Tracks all Alium SmartChef (also known as Pools) contract, with related tokens.

7. **[Trading Competition v1](https://thegraph.com/explorer/subgraph/alium-official/trading-competition-v1)**: Tracks all metrics for the Easter Battle (April 07—14, 2021).

## v1

To access subgraphs related to Alium v1 ecosystem use [`v1`](https://github.com/Alium-Finance/alium-subgraph/tree/v1) branch.

## To setup and deploy

For any of the subgraph: `blocks` as `[subgraph]`

1. Run the `yarn run codegen:[subgraph]` command to prepare the TypeScript sources for the GraphQL (generated/*).

2. Run the `yarn run build:[subgraph]` command to build the subgraph, and check compilation errors before deploying.

3. Run `graph auth https://api.thegraph.com/deploy/ '<ACCESS_TOKEN>'`

4. Deploy via `yarn run deploy:[subgraph]`.
