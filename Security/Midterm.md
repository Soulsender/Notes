## Frameworks
#### CIA
- Confidentiality
- Integrity
- Availability
- Non-Repudiation
#### NIST
1. Identify
2. Protect
3. Detect
4. Respond
5. Recover
#### 7 Layers
1. Physical
2. Perimeter
3. Network
4. Endpoint
5. Application
6. Data
7. Critical Assets/Users
#### Manageable Network
1. Prepare to document
2. Map the network
3. Protect
4. Reach (accessibility)
5. Control
6. Patch Management
7. Baseline Management
8. Documentation
## Email Security
#### SEG (secure email gateway) blocks unwanted messages
- Cisco secure email
- FortiMail secure email gateway
- Microsoft exchange online protection
#### Email Authentication
- Email authentication stops unauthorized parties from sending email from domains they do not own
	- **DKIM (domain keys identified mail)**
		- signs emails from their domain using public keys
		- public keys are stored in DNS text record
	- **SPF (sender policy framework)**
		- DNS text record that lists IPs of servers that are allowed to send emails
	- **DMARC (domain based message authentication reporting and conformance)**
		- tells receiving email servers what to do after SPF and DKIM
		- can quarantine emails or deliver them
		- can also be used to send the marked emails to admins
		- DMARC policies are stored in DNS text records
## VPN
#### PPTP (point to point tunneling protocol)
- microsoft proprietary
- TCP/IP only (port 1723)
- outdated and vulnerable
#### L2F (layer 2 forwarding)
- cisco proprietary
- operates at layer 2
- does not encrypt data
- w/ PPTP it is L2TP