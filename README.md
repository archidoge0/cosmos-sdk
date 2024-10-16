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

# Audit Reports
The following audit reports are available for Cosmos-SDK and the Nubit DA network:
- [Nubit NativeToken Audit (2024)](./docs/audit/Nubit-NativeToken_Audit_2024.pdf) - An audit report specifically covering the adaptations made to the Cosmos-SDK for Nubit’s native token functionalities.
- [Nubit DA General Audit (2024)](./docs/audit/Nubit_DA_Fuzzland_Audit_2024.pdf) - A general audit by Fuzzland, addressing security and operational consistency across the Nubit DA network repositories.