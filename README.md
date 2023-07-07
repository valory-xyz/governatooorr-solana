# Governatooorr Solana

The [Governatooorr](https://governatooorr.autonolas.network/) is an autonomous, AI-powered delegate that votes on on-chain governance proposals on the Etherum and Solana mainnets. This repository lists the software artifacts that make the Solana deployment.

Governatooorr's Solana deployment uses [Autonolas](https://olas.network/), the [Open-AEA](https://github.com/valory-xyz/open-aea) and [Open-Autonomy](https://github.com/valory-xyz/open-autonomy) frameworks and builds on top/interacts with the following Solana-specific components:

* [Governatooorr Solana service](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/services/governatooorr_solana)
* [Governatooorr Solana agent](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/agents/governatooorr_solana)
* [Governatooorr Solana chained skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/governatooorr_solana_abci)
* [Governatooorr Solana proposal collector skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/proposal_collector_solana_abci)
* [Governatooorr Solana proposal voter skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/proposal_voter_solana_abci)
* [Solana transaction settlement skill](https://github.com/valory-xyz/governatooorr/tree/main/packages/valory/skills/solana_transaction_settlement_abci)
* [Solana Open AEA plugin](https://github.com/valory-xyz/open-aea/tree/main/plugins/aea-ledger-solana)
* [Autonolas registries Solana integration](https://github.com/valory-xyz/autonolas-registries/tree/main/integrations/solana): registries for components, agents and services of the autonolas-v1 protocol in its Solana deployment.


# Governatooorr Solana instance deployment

A service instance has been deployed on Solana mainnet, the service owner being the address [deE9943tv6GqmWRmMgf1Nqt384UpzX4FrMvKrt34mmt](https://solscan.io/account/deE9943tv6GqmWRmMgf1Nqt384UpzX4FrMvKrt34mmt).
The registration transaction can be seen [here](https://solscan.io/tx/BCLbNtdX6woJWozcgtRSrvSZxnk8tRUAsrLTmaihXEsS61BvQsWmMoWBE5gUGdk6mvQLUPVHt1HMCG19zTrCSre).

The service operation is governed by a 3-out of-4 multisig that can be found [here](https://solscan.io/account/94jZ2qasXkguDKLWtetTQcZg4rGTpRDPrsR7v2iKDRGt).


# Service Registry Solana program details

The ServiceRegistrySolana program has been created in order to manage on-chain part of the service registry.
The Governatooorr has been created via the ServiceRegistrySolana program.

The program is deployed with the following addresses related to it:
- Program: [AU428Z7KbjRMjhmqWmQwUta2AvydbpfEZNBh8dStHTDi](https://solscan.io/account/AU428Z7KbjRMjhmqWmQwUta2AvydbpfEZNBh8dStHTDi)
- Storage account: [AjHVkc5XV7wiH3KyqznfCGvMofmBQL8agF6HxCjn6H1R](https://solscan.io/account/AjHVkc5XV7wiH3KyqznfCGvMofmBQL8agF6HxCjn6H1R)
- PDA escrow: [Gtb5et18X9b63Yex1wpPtKezeXznqDiqJ3zXh1WAqRxK](https://solscan.io/account/Gtb5et18X9b63Yex1wpPtKezeXznqDiqJ3zXh1WAqRxK)

The program binary is located [here](https://github.com/valory-xyz/autonolas-registries/blob/main/integrations/solana/scripts/ServiceRegistrySolana.so).

The program IDL is located [here](https://github.com/valory-xyz/autonolas-registries/blob/main/integrations/solana/scripts/ServiceRegistrySolana.json).

Once the Governatooorr service is created, these are the steps that were required for its eventual deployment:
- [Registration activation](https://solscan.io/tx/G7JRgwDo1Uaysz5WQ4t7XvbkrpLEdxuTRCUfDHL8LjfHS6Z6Jjdo9NZUMkCzPja1fhDhbnxszXdy6jAMuYe479w);
- [Registration of agent instances](https://solscan.io/tx/5Mdju6f6uqopdjtJswsGmW6A2C1gb55SpLRFZ5MSkAQKg8YfzfE5EUf6jSkuideHSAG7v22hsN7whMjNEEbmN1EM);
- [Service deployment](https://solscan.io/tx/5yNhFGMKvM6ioySEY8AccmrJJ63FQThoD8wnx4mbtBKcS3EN3FpdJZK6JKbgoR4GDNANC6GwydgLR94E7DRHStNt).

The script for creating a service and managing all the steps up to its deployment can be found [here](https://github.com/valory-xyz/autonolas-registries/blob/main/integrations/solana/scripts/mainnet_service_management.js).

Service Registry Solana program development and deployment guidelines can be observed in more details in its integration repository [here](https://github.com/valory-xyz/autonolas-registries/tree/main/integrations/solana).
