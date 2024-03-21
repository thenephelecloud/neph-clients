# Helle (Nephele Beacon Chain) - initially permissioned
TTD: `TBD`  # Set according to the permissioned environment needs

GENESIS_FORK_VERSION: `TBD`  # Determine based on network configuration

ENR for consensus clients:
```yaml
# Example bootnode for illustration
  - "enr:-Ku4QMiLJZSZ-P9K_HJYaOe8YfjkFfY0SoG5bkRY3tp5RePbHcPZGH6Mp5sEgE6FU5tCFMnDH7SGb3nSVfHKHUzPUIBgmlkgnY0gmlwhCLE3VIJc2VjcDI1NmsxoQLH-4uTQOMQjS7D3Vy5HlvpS5fMVCkSh5SMyY8ylCDDdWRwgiMo"
  - "enr:-LK4QDi7DA4diW5NHTBlaPmYZ4jxMfaoJmtRqStGtENShULiS9sghDfXJVgFG5DOnc1HRsFbWeJE8SmPpAxIuD1ohXO4gmlkgnY0gmlwhCJHbVkJc2VjcDI1NmsxoQK5G_VvgHbQlL0V4VS0SHl2THCkMVOaGDLTbfbbGIT4TIaDdWRwgiMo"
# Additional bootnode
    - "enr:-JK4QEzVSLCXX8Nn8kDx9D9mHnHmA84Gjes5dRl9CXRe3XMDIbhrFSCC1MeUJ7Ll-5DMnN7tt6VxG5rS9sZ3HaR1gneDdWRwgiMo"
```

Altair will fork at epoch 50 and merge epoch at 100.
```yaml
genesis_time: TBD  # Set the genesis time for the network
genesis_state_root: TBD  # Initial state root hash
genesis_latest_block_header:
  slot: 0
  proposer_index: 0
  parent_root: 0x0000000000000000000000000000000000000000000000000000000000000000  # No parent since this is the genesis block
  state_root: TBD  # Replace after finalization of the genesis state
  body_root: TBD  # Body root for the genesis block
genesis_block_root_no_state_root: TBD  # Block root without state root update
genesis_block_root_updated_state_root: TBD  # Block root with state root update
genesis_validators_root: TBD  # Root of the validators list at genesis
genesis_validators_count: 6  # For a smaller network of 6 validators
genesis_active_validators_count: 6  # Assuming all are active initially
genesis_total_active_stake_gwei: TBD  # Total active stake in Gwei
genesis_total_balance_gwei: TBD  # Total balance of validators in Gwei
eth1_data:
  deposit_root: TBD  # Deposit contract Merkle root
  deposit_count: 0  # No deposits at genesis
  block_hash: TBD  # Eth1 block hash linked at genesis
deposit index: 0  # Starting index for deposits
genesis_fork_version: TBD  # Fork version at genesis
genesis_fork_digest: TBD  # Fork digest at genesis
pre_genesis_fork_digest: TBD  # Fork digest before genesis
```

Key <> client team mapping for the smaller network could be simplified:
```
EF: 0-0
Nethermind: 1-1
Besu: 2-2
Erigon: 3-3
Lighthouse: 4-4
Teku: 5-5
```
