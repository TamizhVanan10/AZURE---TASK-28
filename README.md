# AZURE---TASK-28

### Implement Traffic Management


. Create Virtual Networks (VNet)

Hub VNet: Create a Virtual Network for the hub in the central region.

Spoke VNets: Create separate Virtual Networks for each spoke (each VNet in different regions or within the same region).

. Configure Subnets
. 
In each VNet (hub and spokes), configure required subnets (e.g., Front-end, Back-end, Gateway, etc.).

. Set Up VNet Peering
 
Hub to Spoke Peering: Peer the hub VNet with each spoke VNet.

Spoke to Spoke Peering (optional): If needed, peer spokes with each other through the hub.

. Configure Network Security Groups (NSGs)
   
Apply NSGs to control traffic flow between the subnets, VNets, and across the hub-spoke model.

 Set Up Azure Firewall or Network Virtual Appliances (NVA)

Deploy Azure Firewall or NVA in the hub VNet to manage traffic between hub and spokes.

 Route Traffic via Hub
 
Configure User-Defined Routes (UDRs) to direct traffic from spokes to the hub for centralized management.

. Enable Shared Services (Optional)
Optionally, deploy shared services in the hub VNet (e.g., DNS, AD DS) that can be accessed by the spokes.

. Monitor and Manage Traffic
    
Use Network Watcher and Azure Monitor to monitor traffic flow and troubleshoot issues in the hub-and-spoke network.

This sets up a secure, scalable traffic management system for your Azure resources using a hub-and-spoke topology.




