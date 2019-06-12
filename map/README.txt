# This directory should contain some mapping contents relative to informing topological design of the AutoSBCL approach.

Given: A user needs to conduct a merge_request
When: The Given Project is on a relative upstream branch target
Then: Merge target branch should be pushed into a temporary testing branch for unit testing
When: that unit testing completes and passes
Then: A binary build shall be queued
When: that binary build completes
Then: that binary build should be pushed to narcissus
When: that binary build is built into OpenStack
Then: An integration test across the SBCL should be run
