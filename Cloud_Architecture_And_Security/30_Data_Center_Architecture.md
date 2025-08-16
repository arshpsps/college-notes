#### Switches

Redirects data to the intended port / device

##### Layer 2 Switch

- Data Link Layer
- Uses MAC address to determine where to send data

##### Layer 3 Switch

- Network Layer
- Uses IP address to route data
- Can use MAC address - Layer 2

#### Hub

Rebroadcasts data from a source to all devices.

#### Router

Routes / forwards data from on network to another based on their IP address.

---

#### Racks

- Width: 19 / 21 inches, universally agreed / not a standard
- Height: **1U** - 1.75 Inches
- most switches & routers take up 1U but other devices like storage arrays can take up more (3U, 4U, etc)
- Rack Sizes: 48U, 42U, 36U, etc
- Can mount monitors, keyboards, UPSs, etc

We leave space in between (usually middle of rack) the devices for cooling.

##### Subracks

Storage devices mounterd on racks that themselves house other passive / active equipment.
also called chasis

##### Top of Rack (TOR) switch

- mostly leaf in a spine-leaf architecture
- network switches that connect the entire entwork of the servers / storage on a rack

###### Benefits:

- Copper cabled stay in rack.
- Reduced cabling costs per rack.
- modular and flexible per rack architecture.
- future proofing for higher speeds.

#### [Datacenter](https://www.youtube.com/watch?v=ukBPwRluwSQ&t=65s)

##### Spine-leaf Architecture

**Spine**: These are the top / higher level switches that the leaf switches connect to. These route traffic between leafs.

**Leaf**: It's basically a node. This switch connects directly to servers, storage & other devices and forwards all this traffic to the spine.

##### Traffic

###### North-South Traffic

Data that is **external** to the datacenter.

If data travelling between datacenters goes through a public network, it is considered North-South.

This is traffic that comes in or goes out of a data center to outside world.

- **Southbound**: Traffic entering a datacenter.
- **Northbound**: Traffic exiting a datacenter

###### East-West Traffic

Data that is **internal** to the datacenter.

If data travelling between datacenters goes through a private network, it is considered East-West.

Traffic moving between machines inside a datacenter.

##### Meet Me Room

A central point where equipment connevtivity converges.

##### Tiers

- Range 1 to 4
- worst (1) to best (4)

**Factors**:

- Service Availability & uptime guarantees
- Redundancy level
- Cooling & Power Level
- Datacenter security level
- Staff experties & Maintenance level
- Service Cost

---

#### Demilitarized Zone (DMZ)

Network/"buffer zone" where security policies are relaxed.

- Used to isolate a network that connects public and private networks.
- separate network for publically facing services.
