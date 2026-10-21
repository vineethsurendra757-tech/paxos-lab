# Fundamentals of System Security (COMSM0122)
## Workshop 3: Understanding and Stress-Testing Paxos

### Author Information
* **Name:** Vineeth Surendra
* **Degree:** MSc Cybersecurity, University of Bristol

---

## Overview
This repository contains an educational JavaScript-based Paxos consensus simulator designed to demonstrate how distributed systems achieve agreement despite node crashes, state loss, network partitions, and misconfigurations. It models the core roles—Proposers, Acceptors, Learners, Quorums, Proposal Numbers, and Network Exchanges—to explore protocol safety, liveness, and operational hardening.

---

## Directory Structure
```text
paxos-lab/
├── package.json
├── simulator.js
├── proposal.js
├── proposer.js
├── acceptor.js
├── learner.js
├── quorum.js
├── network.js
├── assumption_failures.js
└── scenarios/
    ├── happy_path.js
    ├── acceptor_failure.js
    ├── competing_proposers.js
    ├── partial_acceptance.js
    ├── preserve_chosen_value.js
    ├── multi_paxos.js
    ├── network_partition.js
    └── breaking_assumptions/
        ├── majority_loss.js
        ├── state_loss.js
        ├── quorum_misconfiguration.js
        └── hardening.js


    ###Installation
    Install project dependencies:
    Bash
    npm install
    
    Running Scenarios
    To run any of the workshop scenarios, use the corresponding npm command:
    
    Bash
    npm run happy          # Part 1: Happy Path Consensus
    npm run failure        # Part 2: Acceptor Failure
    npm run proposers      # Part 3: Competing Proposers
    npm run partial        # Part 4: Partial Acceptance
    npm run preserve       # Part 5: Preserving Chosen Values
    npm run multi          # Part 6: Multi-Paxos
    npm run partition      # Part 7.1: Network Partitioning
    npm run majority-loss  # Part 7.2: Majority Loss
    npm run state-loss     # Part 7.3: State Loss
    npm run quorum-error   # Part 7.4: Quorum Misconfiguration
    npm run hardening    # Part 8: Hardening Paxos Deployment

