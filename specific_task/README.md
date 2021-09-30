# Scale Computing System REST API Examples - Task Specific

This repository contains scripts for running task-specific API queries against a Scale system.

These scripts are only examples and demonstrate common use cases with the API.  
Refer to the API docs on a scale system for a detailed guide on available calls.


### SnapshotReport.ps1

Returns the latest replication snapshot that falls outside of a defined age timeframe.
Includes optional arguments to retrieve additional information about snapshots, schedules,
and remote cluster connections.


### checkAffinity.ps1

Provides the LAN IP addresses and uuid values for each node in the target cluster for quick
reference. Also provides each VM, the present node location of the VM, and the preferred 
and backup affinity assignments.

### SetTag.ps1

Sets the VM tag value using a VM name string with an optional ability to restart the VM.
Useful for applying any tag, but especially for applying a GPU tag and restarting the VM
to enable the vGPU.
