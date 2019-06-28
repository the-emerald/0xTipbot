# Roadmap
Note: Some ideas are taken from 0x1d00ffff. Thanks!

Bot has a single priv/pubkey, all balances are in one account and bookkeeping can be done using a db.

## Depositing
1. The user binds a discord user ID (theirs) to an Ethereum address.
2. The user is free to deposit any tokens to the tipbot wallet address.
3. Every X minutes the tipbot checks the address for incoming transactions from that address
Note: Tokens that are not yet implemented / tokens deposited from a new address will need to be rescued manually.

## Tipping
Note: 'Tipping' here describes the `!tip` command, which only tips one user.
1. The tip command is evoked and some sanity checks are made.
2. The tip is executed off-chain.

## Withdrawl
1. The user creates a withdrawl request, specifying the token and price they want to use as payment for the lava pocket
2. The packet is generated and sent off to relayers.
