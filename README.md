## Azure Networking Lab

### Architecture
- Resource Group: rg-network-lab
- Virtual Networks:
  - vnet-app
  - vnet-secure
- Peering configured between VNets

### Security
- NSG applied to subnet
- SSH allowed only via controlled rule
- No open public access between VMs

### Virtual Machines
- vm-web (inside vnet-app)
- vm-secure (inside vnet-secure)

### Connectivity Test
- SSH from vm-secure → vm-web using private IP
- Key-based authentication used
- Verified successful internal communication

### Result
Secure communication between isolated networks using Azure VNet peering and NSG rules.
