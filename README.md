# Governatooorr Solana

The [Governatooorr](https://governatooorr.autonolas.network/) is an autonomous, AI-powered delegate that votes on on-chain governance proposals on the Etherum and Solana mainnets. The Ethereum version is already deployed, and will be followed by the Solana deployment.

Governatooorr uses [Autonolas](https://olas.network/), the [Open-AEA](https://github.com/valory-xyz/open-aea) and [Open-Autonomy](https://github.com/valory-xyz/open-autonomy) frameworks and builds on top/interacts with the following components:

* [Governatooorr Solana service](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/services/governatooorr_solana)
* [Governatooorr Solana agent](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/agents/governatooorr_solana)
* [Governatooorr Solana chained skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/governatooorr_solana_abci)
* [Governatooorr Solana proposal collector skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/proposal_collector_solana_abci)
* [Governatooorr Solana proposal voter skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/proposal_voter_solana_abci)
* [Solana transaction settlement skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/solana_transaction_settlement_abci)
* [Solana Open AEA plugin](https://github.com/valory-xyz/open-aea/tree/main/plugins/aea-ledger-solana)
* [Autonolas registries Solana integration](https://github.com/valory-xyz/autonolas-registries/tree/main/integrations/solana): registries for components, agents and services, the second part of the autonolas-v1 protocol.