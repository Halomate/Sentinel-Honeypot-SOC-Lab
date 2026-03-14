# Attack Investigation

After exposing the Azure virtual machine to the public internet, automated attacks began within minutes.

The following activity was observed:

- Repeated RDP login attempts
- Automated password guessing attempts
- Login attempts from multiple global IP addresses

Using Microsoft Sentinel, failed login events were analyzed using KQL queries.

Event ID 4625 was used to identify authentication failures.

Attackers were identified by analyzing the IPAddress field and mapping it to geographic locations.

Example attack activity:

- Multiple failed logins from the same IP
- Repeated authentication attempts within short time windows
- Global scanning behavior from automated bots

This demonstrates how quickly publicly exposed systems are targeted by automated attacks.
