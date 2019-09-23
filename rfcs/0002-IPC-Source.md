# Title
* Date: 09/23/2019
* Author: Danny Browning <bdbrowning2@gmail.com>

## Summary

Provide a source for sharing packets via IPC (Shared Memory), that can be used as a library.

## Motivation

A number of users have asked for "suricata as a library". Part of this functionality is already provided via EVE outputs, but there is no equivalent for sharing packets with suricata. FIFO pipes are one possibility, but as workloads increase, may produce undesirable blocking behavior on either side of the pipe.

## Proposal

Provide a new source, which can take in a number of ipc (shared memory) channels to provide for multi threaded capture and analysis of packets from a source external to suricata.

## References

* [Example IPC Source](https://github.com/dbcfd/packet-ipc)
* [Underlying Shared Memory Mechanism](https://github.com/servo/ipc-channel)
* [Single Channel Implemntation](https://github.com/dbcfd/suricata/tree/sensicata)
