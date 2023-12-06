# Jarkom-Modul-4-I05-2023

## Modul 4 Jarkom 2023 I05 Formal Report

Group Members:
| No |  Name    |  NRP  |
| ---       |   ---     |---  |
|     1     |     Khairiya Maisa Putri    | 5025211192 |
|     2     |     Talitha Hayyinas Sahala    |  5025211263 |

Method that we are using: GNS - CIDR and CPT - VLSM

## Prefix IP
Our Prefix IP `10.61`

## Topologi GNS CIDR
![TopologiGNS](img/topologiGNS.png)

## Topologi CPT VLSM
![TopologiCPT](img/topologi-vlsm.png)

## Route
After doing research and conducting experiments and seeing how to `route` the Jarkom module, the results of the routes we got are as follows

![Route](img/route.png)

## VLSM

In English, the translated text would be:

VLSM, commonly known as `Variable Length Subnet Masking`, is a `subnetting` technique used to optimize the distribution of `IP addresses` within a network. The `size` of the `netmask` is adjusted based on the number of computers/hosts that require IP addresses.

In a subnet. By using `VLSM`, we can allocate `IP address` blocks that match the needs of each subnet without adhering to uniform limitations. This allows network administrators to be more flexible in optimizing the use of IP addresses and avoiding resource wastage.

The implementation process of `VLSM` involves breaking down a large network into smaller subnets with varying sizes. Each `subnet` is then assigned a netmask according to the number of hosts required within it. In this way, subnets that require more hosts will have a netmask with fewer bits, while subnets needing fewer hosts will have a `netmask` with more bits.

The main advantage of `VLSM` is the efficient use of IP addresses, as it allows us to avoid assigning large-sized subnets to small networks that actually require only a small number of IP addresses. Additionally, VLSM aids in reducing overall IP address consumption in the network, thereby supporting growth and expansion more `effectively`.


**VLSM TREE**

The following is the result of `breaking down` a large subnet which will be formed into a smaller `network`

![VLSMTREE](img/VLSM_TREE.png)

**IP VLSM**

The following are the results of dividing the `IP` that we obtained from the `split` into smaller networks

![IPVLSM](img/IP-VLSM.png)


## CIDR
### Merging Subnets
The first thing that we need to do is to **merged** the subnets from the furthest one from the internet, untill all of the subnets merged into one.

**Initial State**
![initial](img/awal.png)

**First Merge (B)**
![first](img/pertama.png)

First merging table:
![b](img/B.png)

**Second Merge (C)**
![second](img/kedua.png)

Second merging table:
![c](img/C.png)

**Third Merge (D)**
![third](img/ketiga.png)

Third merging table:
![d](img/D.png)

**Fourth Merge (E)**
![fourth](img/keempat.png)

Fourth merging table:
![e](img/E.png)

**Fifth Merge (F)**
![fifth](img/kelima.png)

Fifth merging table:
![f](img/F.png)

**Sixth Merge (G)**
![sixth](img/keenam.png)

Sixth merging table:
![G](img/G.png)

**Seventh Merge (H)**
![seventh](img/ketujuh.png)

Seventh merging table:
![h](img/H.png)

**Eighth Merge (I)**
![eighth](img/kedelapan.png)

Eighth merging table:
![i](img/I.png)

### IP Tree
From the merging process above, we will get an IP **tree** like down below:

![tree](img/tree.png)

### IP Divisions
Based on the IP tree above, we can divide the IP for each subnets, where we can count the broadcast IP by implementing the OR operation on IP and inverted netmask. And we will get there IP Broadcasts for each subnets:

![pembagian](img/pembagian.png)
