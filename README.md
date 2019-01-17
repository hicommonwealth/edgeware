# edgeware
Edgeware is a new, actively governed blockchain. Edgeware fits into the ecosystem as a testnet for sound, compelling technology that will improve our ability to build robust blockchain technology. We accomplish this with the following:
1. Edgeware is built on substrate and has real, non-trivial value.
2. Edgeware extends substrate with a variety of governance modules such as identity, voting, and novel economic mechanisms.
3. Edgeware will experiment with new governance ideas, deploying them quicker than larger, more established protocols.
4. Edgeware open-sources these technologies and experiments as well as a variety of UI/UX tools for interacting with governance.

Together with these tenets, Edgeware stands to improve the approach to blockchain governance by numerous orders of magnitude. We can efficiently experiment with new ideas, publish results, and inform the general ecosystem about improvements or degradations in thought processes.

The edgeware client: [edgeware-node](https://github.com/hicommonwealth/edgeware-node)

## Modules
Edgeware is an specialization of a substrate chain. The following list details the modules of Edgeware as they relate to substrate's runtime module library.

#### edge_identity
The identity module handles registration, attestation, and claims issuance for identities. Identity is paramount for a variety of voting protocols and is a core focus of Edgeware's approach to offering as many governance primitives as possible.

- [edge_identity](https://github.com/hicommonwealth/edge_identity)

#### edge_delegation
The delegation module handles delegation of voting weight, which can be denominated using any pricing rule. These pricing rules can be 1 identity 1 vote, 1 coin 1 vote, and even quadratic voting. The purpose of this module is to provide a decoupled interface for any existing and future module to take advantage of delegation in a voting mechanism.

- [edge_delegation](https://github.com/hicommonwealth/edge_delegation)

#### edge_governance

The governance module contains the logic that powers Edgeware's governance UI. It is presented as a broader governance module that forms something akin to a forum for governance proposals. Users can submit proposals, vote on proposals, and track progress of proposals through Edgeware's governance process.
