Network Summary:

The network is organized into two primary VLANs: one for general employees and another for 
the Security Operations Center (SOC). Each VLAN operates on its own layer 2 switch, both of 
which are linked through a central layer 3 switch. This layer 3 switch connects to a router, which 
then links to a firewall. The firewall is positioned before the edge router that interfaces with the 
external network.

Firewall Policy Approach:

By default, all traffic is blocked unless explicitly allowed. Access is only granted for HTTP and 
HTTPS connections to a list of approved and trusted IP addresses. A strict least privilege model 
should be enforced for all users and systems, ensuring that only the necessary permissions are 
granted. This approach helps prevent both external threats and internal risks, such as users 
unintentionally or intentionally accessing unauthorized data.

Security Containment Strategy:

Blocking all unspecified traffic reduces the chance of external attacks reaching the internal 
network. The least privilege principle further protects sensitive information by restricting access 
based on necessity.

Monitoring Support:

The firewall configuration improves monitoring by working in tandem with intrusion detection 
systems (IDS) and a Security Information and Event Management (SIEM) solution.

Conclusion:

Apply a deny-by-default firewall policy, allow only essential traffic, enforce least privilege 
across the network, and integrate monitoring tools like IDS and SIEM for effective threat 
detection and response.
