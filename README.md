# Sawtooth PBFT

This repository contains an implementation of the Practical Byzantine Fault
Tolerant (PBFT) consensus algorithm for
[Sawtooth](https://github.com/splintercommunity/sawtooth-core).

## About PBFT

PBFT is designed to tolerate the failure of nodes in a distributed network,
as well as nodes sending incorrect messages to other nodes, as long as fewer
than one-third of the nodes are considered faulty. PBFT networks need a minimum
of four nodes to be Byzantine fault tolerant.

Sawtooth PBFT is based on the algorithm described in [Practical Byzantine Fault
Tolerance](https://www.usenix.org/legacy/events/osdi99/full_papers/castro/castro_html/castro.html),
and is adapted for use in Sawtooth.

For more information, see the [Sawtooth PBFT
documentation](https://sawtooth.splinter.dev/docs/1.2/pbft/introduction-to-sawtooth-pbft.html).

## Using Sawtooth PBFT Consensus

To configure a Sawtooth network with PBFT consensus, see the Sawtooth
documentation:

- Application developers: [Creating a Sawtooth Test
  Network](https://sawtooth.splinter.dev/docs/1.2/app_developers_guide/creating_sawtooth_network.html)

- System administrators: [Setting Up a Sawtooth
  Network](https://sawtooth.splinter.dev/docs/1.2/sysadmin_guide/setting_up_sawtooth_network.html)

## Motivation

PBFT was chosen as a Sawtooth consensus algorithm in order to provide
Byzantine fault tolerant consensus for a system without a Trusted Execution
Environment (TEE). (PoET-SGX consensus requires a TEE.)

The proposal to include PBFT in Sawtooth is located in [Sawtooth RFC
0019-pbft-consensus.md](https://github.com/splintercommunity/sawtooth-rfcs/blob/main/text/0019-pbft-consensus.md).

Sawtooth PBFT uses the Sawtooth consensus API that is described by [Sawtooth RFC
0004-consensus-api.md](https://github.com/splintercommunity/sawtooth-rfcs/blob/main/text/0004-consensus-api.md).

## Documentation

- [Current Sawtooth PBFT documentation](https://sawtooth.splinter.dev/docs/1.2/pbft/introduction-to-sawtooth-pbft.html)

## License

Sawtooth software is licensed under the Apache License Version 2.0
software license.
