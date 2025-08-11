#### RAID - Redundant Array of independent Disks

Data is copied in multiple disks to prevent data loss.

##### RAID 0

Data is split across multiple disks. (NOT COPIED, SPLIT)
So, there is only a single copy of the data.

NOT Fault Tolerant.
Speed Advantage

##### RAID 1

Data is copied on more than 1 Disks.

IS Fault Tolerant.
Each disk has same data.

##### RAID 5

Data is split across multiple disks. Some thing called **parity** is also stored on these disks.

IS Fault Tolerant
But, it can handle only 1 disk failure at a time

###### Parity

**parity** is data used to rebuild the data in case of loss.
Parity takes up the equivalent of an entire disk's space.

Let's say Disk A and Disk B store actual data. Disk C is used for parity.

Disk A XOR Disk B = Parity

```
1   1   0
0   0   0
0   1   1
1   0   1
A   B   C
```

Let's say we lost the entirety of Disk B.
We could rebuild data of Disk B from Disk A XOR Disk C (Parity Disk)

```
1   0   1
0   0   0
0   1   1
1   1   0
A   C   B
```

We do the exact same XOR across multiple disks if there are more.

##### RAID 10 - 1+0

Combines RAID 1 with RAID 0

Required minimum of 4 disks.
Set of 2 disks contain cloned data, this is a group. (RAID 1)

Data is split across group like in RAID 0.

```
            0
    1               1
A       A       B       B
C       C       D       D
E       E       F       F
G       G       H       H
```

Numbers are RAID versions.
Letters are disks.

Only 50% of storage capacity is data, rest is clone.
