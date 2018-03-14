# XOSAN creation guide

## Prerequisites

XOSAN will need a pool with:

* XenServer 7 or higher
* Local LVM SR with at lease 15GiB of free space on **each** host
* 2 GiB of free RAM on each host for the XOSAN VM
* A working connection with the updater (same way as the XO trial)
* Our XOSAN pack installed on each hosts (it's automatically deployed during the first XOSAN install)

> The pack will install user-space packages and add a new SR type: "xosan". Their will be no other modification. The tool stack has to be restarted to be able to deal with XOSAN (no VM or service interruption). It's also fully automated in the XOSAN install process.

### Optional

* An extra/dedicated physical network for storage to deliver high performances
* 10G networks will deliver higher throughput

## Creation

After the completion of all the requirements, you can install XOSAN itself.

1. Select all local SR you want to participate to the new shared SR
2. Choose the mode you want to use. Disperse or replicate which will allow you to lose one or many host without experiencing data loss. To get more information about the XOSAN modes, check our documentation
3. That's it! Your XOSAN is now ready to be used.
