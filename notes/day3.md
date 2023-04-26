# Scaling

- Layer 1 approaches
- Different consensus mechanism
  - Proof of stake
  - Proof of history
- Sharding
- Layer 2 approaches (off-chain scaling)
- Rollups
  - Fuel
  - Optimism
  - Aztec
  - Starkware
- Sidechains
  - xDAI
- State channels
  - Raiden (equivalent to bitcoin lightning network)
  - Connext
  - Perun
- Plasma
  - Matic
  - OMG
  - Gluon
- Validium
  - StarkEx

# Rollup

- Transaction execution outside layer 1
- Data or proof of transactions is on layer 1
- A smart contract on layer 1 is used to verify correct transaction execution by using the data on layer 1
- Main chain holds funds & commitments to the side chains
- Side chains hold the state & performs execution
- Needs to be a proof
  - Fraud proof or
  - Validity proof
- Operators/Sequencers performs the transaction, bundles them & submits the proof to the main chain
  - They have to stake a bond to ensure they are honest. Dishonesty leads to slashing of the bond
- Two types of rollups currently:
  - Optimistic
    - Submits with bare information
    - Proofs are submitted only when a fraud is detected
  - ZK
    - Two types of users
      - Transactors
        - Create their transfer and broadcast the transfer to the network
      - Relayers
        - Collect the transfers and create a rollup & generate the snark proof
        - They have to stake to become a relayer

# Applications of zk in the wild

- FileCoin
- Zcash
- Monero
- TornadoCash
- DarkForest