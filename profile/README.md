Gas Killer is a verifiable off-chain compute service that reduces gas costs for complex EVM transactions.

Smart contracts that perform expensive computations (storage updates, aggregations, simulations) can offload that work to the Gas Killer AVS. A network of EigenLayer operator nodes validates and signs each task. The router aggregates their BLS signatures and, once a threshold is reached, submits a single `verifyAndUpdate` transaction onchain with a compact proof instead of executing the full computation there.

The result: predictable, low-gas writes for contracts that would otherwise be too expensive to call.
