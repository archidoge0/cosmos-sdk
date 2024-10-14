# cosmos-sdk

Cosmos-sdk [cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk) offers a framework for building blockchain applications with CometBFT consensus.

This repo is a fork of cosmos-sdk v0.46.16 (v0.46.x) with adaptions.

# Modifications
1. Adoption of PrepareProposal and ProcessProposal
1. The addition of chainID to baseapp so that a branch of state can be used in PrepareProposal and ProcessProposal
1. The addition of  `--btc-rpc` parameter that enables the program to retrieve the current BTC block height.
1. Increase `DefaultPowerReduction` from `1000000` to `100000000`

# Contributing
This repo intends on preserving the minimal possible diff with [cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk) to make fetching upstream changes easy. If the proposed contribution is
- specific to Nubit: consider if [nubit-validator](https://github.com/RiemaLabs/nubit-validator) is a better target
- not specific to Nubit: consider making the contribution upstream in [cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk)