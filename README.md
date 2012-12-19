VISON
=====

Visibility Initiative, Statewide Owned Network

Documented scripts and processes for

1. Creating a state blessed, CIS hardened, CentOS network server. 
2. Configure a VPN-like tunnel back to a central location for feeding alert data
3. enable and configure locally unique rules for Snort, Ntop, Syslog-ng, OSSEC
4. automate installation of root components using a State Vetted Local repository for server components 


Specifically excluded components from this public repository:
1. Keypairs
2. sensor config customizations

Contact michael.miller at state dot co dot us for questions or concerns, alternately, try mike-VISON at millertwinracing dot com




=========
Build notes

Sensor Deployment VISN

DOCUMENTATION
IS this CentOS centric? (possibly not)
All scripts should accept, cleanly, additional installs. 
Need to have unidirectional signalling scripts to update sensors
Any Cloud-centric considerations?
CIS Hardened
Github
Chef
Centos
Central Repository for software, configs, etc (NOT GITHUB - Info leak)
Certificate Membership Based - Different per Machine or shared?
Management Virtual Network
Snort
Pulled Pork
pOf
Sensor Stats Reporting - dropped packets, etc. 
Ntop
Syslog - Append location Specific fingerprints, nightly log rotate and compress, 
OSSEC - report issues back to Server Host
Must have reporting service - Mail (standalone?)
Feed results to Qradar (what and how much is necessary?)

Server Host….redundant? Load Balanced?
  RFC1918 - obfuscate discovery from external haxx0rs

Security layout:
	sudo has access to all
		DataVault has access to data, that section has Execute privs turned off
		(Some way to remove chmod?)
		Chroot jail?
