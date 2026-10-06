# Awesome-Virtual-Private-Cloud-Vpc-Networking

## Top Virtual Private Cloud (VPC) Networking Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cloud Network Isolation, Overlay Networking & Self-Hosted SDN*  

**Last updated: October 2026**



This repository tracks notable **commercial VPC platforms** and **open-source projects** that create isolated, private networks within public clouds and self-hosted infrastructure. These tools provide network segmentation, routing, firewalling, and connectivity between cloud resources — the foundation of cloud security architecture.



**Examples** include Amazon VPC, Azure Virtual Network, Google Cloud VPC, DigitalOcean VPC, Linode Cloud VPC, Vultr VPC 2.0, OVHcloud vRack, Scaleway Private Networks, Hetzner Cloud Networks, and Alibaba Cloud VPC (the category leaders).



**Open-source emphasis**: VPC networking is a strong open-source domain. **Open vSwitch** and **OVN** provide the virtual switching and logical networking foundation. **Cilium** and **Calico** bring eBPF-based networking and security to Kubernetes. **Netmaker**, **NetBird**, **Tailscale**, and **Headscale** deliver WireGuard-based overlay networks. **ZeroTier** provides multi-cloud SDN. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Amazon VPC](https://aws.amazon.com/vpc/)**  

  **The reference implementation for cloud VPC** — full control over IP addressing, subnets, route tables, and gateways. **The industry standard** with extensive third-party tooling and documentation.



- **[Azure Virtual Network](https://azure.microsoft.com/en-us/products/virtual-network/)**  

  Microsoft's foundational VPC service — isolated network segments with subnets, NSGs, and peering. **Native integration with Azure services and hybrid connectivity** via VPN Gateway and ExpressRoute.



- **[Google Cloud VPC](https://cloud.google.com/vpc)**  

  GCP's global VPC with automatic subnet creation, global routing, and native integration with Google services. **Supports shared VPC** for multi-project organizations.



- **[DigitalOcean VPC](https://www.digitalocean.com/products/vpc)**  

  **Simple, free VPC networking** — private networking between Droplets in the same region. **Free with DigitalOcean** — no additional cost .



- **[Linode Cloud VPC](https://www.linode.com/products/vpc/)**  

  **Free VPC networking** — private network segments for Linode instances. **Free with Linode** — no additional cost .



- **[Vultr VPC 2.0](https://www.vultr.com/features/vpc/)**  

  Vultr's VPC networking — private networking across instances and regions. **Free with Vultr** .



- **[OVHcloud vRack](https://www.ovhcloud.com/en/network/vrack/)**  

  **Private network across OVHcloud products** — connect dedicated servers, VPS, and cloud instances. **The best for hybrid OVHcloud deployments** .



- **[Scaleway Private Networks](https://www.scaleway.com/en/vpc/)**  

  Scaleway's VPC — private networking with regional isolation. **Best for European data sovereignty** .



- **[Hetzner Cloud Networks](https://www.hetzner.com/cloud)**  

  **Private networking for Hetzner Cloud** — connect servers via private IPs. **Free with Hetzner Cloud** .



- **[Alibaba Cloud VPC](https://www.alibabacloud.com/product/vpc)**  

  Alibaba's VPC — isolated networks for Alibaba Cloud resources. **Best for Asia-Pacific deployments** .



## Open-Source GitHub Projects



### Overlay Networking (WireGuard-Based)



- **[Netmaker](https://github.com/gravitl/netmaker)**  

  **The leading open-source WireGuard-based Zero Trust networking platform**, Apache-2.0 licensed with **10,000+ GitHub stars** . **Creates flat, encrypted overlay networks** — every node is "next door" regardless of physical location . **Kernel WireGuard for superior performance** . **Gateways for traffic relaying, security policies with IDP integration, and egress routing** . **The de facto open-source VPC alternative for connecting distributed resources** . **Best for multi-cloud and hybrid cloud networking** .



- **[NetBird](https://github.com/netbirdio/netbird)**  

  **Open-source Zero Trust networking platform**, Apache-2.0 licensed . **WireGuard-based peer-to-peer overlay networks** . **Identity provider integration for granular access control** . **Self-hosted with admin dashboard** . **Best for teams wanting managed-like experience with full data ownership** .



- **[Tailscale](https://github.com/tailscale/tailscale)**  

  **The easiest WireGuard-based mesh VPN**, BSD-3-Clause licensed (client only; coordination server proprietary) . **Excellent NAT traversal, MagicDNS, ACLs, and SSO** . **Best for easy overlay networking** .



- **[Headscale](https://github.com/juanfont/headscale)**  

  **Self-hosted Tailscale control server**, BSD-3-Clause licensed . **Use Tailscale clients with your own coordination server** . **The best combination of speed, security, and vendor independence** . **Best for Tailscale without vendor dependency** .



- **[ZeroTier](https://github.com/zerotier/ZeroTierOne)**  

  **Multi-cloud SDN platform**, BSL 1.1 licensed (client open source; controller source-available) . **Custom protocol with strong NAT traversal** . **True self-hosting requires third-party controllers** . **Best for legacy SDN deployments** .



- **[Gluetun](https://github.com/qdm12/gluetun)**  

  **VPN client with WireGuard and OpenVPN support** — not VPC per se, but provides secure network connectivity . **Best for VPN connectivity** .



### Virtual Switching & SDN



- **[Open vSwitch](https://github.com/openvswitch/ovs)**  

  **Production-quality multilayer virtual switch**, Apache-2.0 licensed . **The foundation for software-defined networking** — used by OpenStack, Kubernetes, and countless SDN projects . **Supports OpenFlow, VXLAN, GRE, and other tunneling protocols** . **The de facto standard for virtual switching** . **Best for building custom SDN infrastructure** .



- **[OVN (Open Virtual Network)](https://github.com/ovn-org/ovn)**  

  **Open-source logical network abstraction for Open vSwitch**, Apache-2.0 licensed . **Adds native support for virtual network abstractions** — logical switches, routers, and ACLs . **Used by OpenStack and Kubernetes** . **Best for cloud-native SDN** .



- **[Cilium](https://github.com/cilium/cilium)**  

  **eBPF-based networking, security, and observability for Kubernetes**, Apache-2.0 licensed with **20,000+ GitHub stars** . **The leading Kubernetes CNI** — provides network policies, service mesh, and multi-cluster networking . **Best for Kubernetes networking and security** .



- **[Calico](https://github.com/projectcalico/calico)**  

  **Open-source networking and security for containers and Kubernetes**, Apache-2.0 licensed . **Network policies, encryption, and observability** . **Best for Kubernetes networking** .



- **[Flannel](https://github.com/flannel-io/flannel)**  

  **Simple overlay network for Kubernetes**, Apache-2.0 licensed . **The simplest CNI** — VXLAN, host-gw, and wireguard backends . **Best for simple Kubernetes networking** .



- **[Kube-OVN](https://github.com/kubeovn/kube-ovn)**  

  **OVN-based Kubernetes networking**, Apache-2.0 licensed . **Advanced networking features** — subnets, QoS, and multi-tenancy . **Best for enterprise Kubernetes networking** .



### Container Networking



- **[Project Calico](https://github.com/projectcalico/calico)** — Already listed. **Enterprise-grade container networking** .



- **[Antrea](https://github.com/antrea-io/antrea)**  

  **Kubernetes networking with Open vSwitch**, Apache-2.0 licensed . **The most mature OVS-based CNI** . **Best for Kubernetes networking with OVS** .



- **[Multus CNI](https://github.com/k8snetworkplumbingwg/multus-cni)**  

  **Multiple network interfaces for Kubernetes pods**, Apache-2.0 licensed . **Attach multiple networks to pods** . **Best for multi-network Kubernetes** .



- **[Submariner](https://github.com/submariner-io/submariner)**  

  **Multi-cluster networking for Kubernetes**, Apache-2.0 licensed . **Connect pods and services across clusters** . **Best for multi-cluster Kubernetes** .



### Infrastructure as Code for VPC



- **[Terraform](https://github.com/hashicorp/terraform)**  

  **Infrastructure as Code standard**, MPL-2.0 licensed . **Provision VPC across providers** — AWS, Azure, GCP, DigitalOcean, and more . **The de facto IaC tool** .



- **[OpenTofu](https://github.com/opentofu/opentofu)**  

  **Open-source Terraform fork**, MPL-2.0 licensed . **Community-driven IaC** . **Best for Terraform without BSL concerns** .



- **[Pulumi](https://github.com/pulumi/pulumi)**  

  **IaC with real programming languages**, Apache-2.0 licensed . **TypeScript, Python, Go, .NET** . **Best for developers wanting IaC in code** .



- **[Ansible](https://github.com/ansible/ansible)**  

  **Configuration management and automation**, GPL-3.0 licensed . **Configure VPC and network devices** . **Best for server configuration** .



### Additional Strong Open-Source Options



- **OpenStack Neutron** — Networking-as-a-Service for OpenStack .

- **OpenDaylight** — Open-source SDN controller .

- **ONOS** — Open Network Operating System .

- **FRRouting** — Open-source routing suite .

- **BIRD** — Internet routing daemon .

- **WireGuard** — Modern VPN protocol underlying most overlay networks .

- **OpenVPN** — Veteran open-source VPN .

- **strongSwan** — IPsec VPN .

- **Libreswan** — IPsec VPN .

- **Tinc** — Mesh VPN daemon .



**Frameworks for building custom VPC solutions**: Combine **Netmaker** for WireGuard-based overlay networking across clouds . Use **Open vSwitch** and **OVN** for building custom SDN infrastructure . Deploy **Cilium** or **Calico** for Kubernetes networking and security . Choose **Terraform** or **OpenTofu** for IaC provisioning . Integrate **Headscale** for self-hosted Tailscale . Note that true commercial VPC with global anycast, managed peering, and enterprise SLAs (AWS VPC, Azure VNet, GCP VPC) remains primarily commercial territory; open-source stacks provide strong overlay networking, virtual switching, and SDN foundations that require integration for complete cloud networking.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- VPC networking handles sensitive network traffic and access control. Self-hosted solutions require proper security hardening, key management, and access policy configuration.

- **Commercial cloud VPCs are free** (AWS VPC, Azure VNet, GCP VPC, DigitalOcean VPC) — you pay for the resources within them, not the VPC itself . Open-source alternatives require infrastructure and operational expertise.

- **Overlay networking introduces complexity** — NAT traversal, key management, and routing require understanding. Netmaker and NetBird simplify but don't eliminate operational responsibility .

- **Kubernetes CNI choice matters** — Cilium, Calico, and Antrea have different performance and feature profiles. Evaluate against your requirements .

- The open-source ecosystem provides strong overlay networking, virtual switching, and SDN foundations, but **global anycast, managed peering, and enterprise SLAs** remain primarily commercial offerings.



---



**Made for network engineers, cloud architects, and organizations seeking VPC networking sovereignty.**  

Let's make virtual private cloud networking more open, transparent, and accessible.
