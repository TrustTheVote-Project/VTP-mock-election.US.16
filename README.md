# A VoteTracker+ Mock US Election Repo

This is a work in progress.

This repository represents the current thoughts on how to configure an election for VoteTracker+.  See the [VoteTrackerPlus](https://github.com/TrustTheVote-Project/VoteTrackerPlus) repository for more information.

## How to clone this and the VoteTracker+ repos and setup up a VTP demo

See the [VTP-dev-env](https://github.com/TrustTheVote-Project/VTP-dev-env) repo for more information.

```bash
# Clone the VTP-dev-env repo, not this repo (https example)
$ git clone https://github.com/TrustTheVote-Project/VTP-dev-env.git

# Run the makefile there, which will pull this and the other repos of interest
# as git submodules of the VTP-dev-env repo.
$ cd VTP-dev-env
$ make init

# Using poetry perform a local install of VoteTracker+
$ cd VoteTrackerPlus
$ make poetry-build

# To setup a mock demo election using this (ElectionData) repo:
$ cd ../VTP-mock-election.US.16
$ setup-vtp-demo
```

See the [developer readme](https://github.com/TrustTheVote-Project/VoteTrackerPlus/tree/main/src/vtp) in the VoteTrackerPlus repo for more details.
