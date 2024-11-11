# Server_Documentation
## To-Do:
- [ ] Hardware
	- [ ] DMZ Router
		- [ ] install NIC
		- [ ] install 1x SSD (Boot Drive)
	- [x] Router
	- [ ] Switch
		- [ ] get Switch
	- [ ] MGMT
		- [ ] install 1x SSD (Boot Drive)
	- [ ] NAS
		- [ ] install 2x SSDs (Boot Drives)
		- [ ] install 4x HDDs (Main Storage Pool)
	- [ ] Gameserver
		- [ ] figure out which drives
			- [ ] install 1x SSD (Boot Drive) 
			- [ ] install 1x SSD (for Gameserver)
			- [ ] install 1x HDD (on machine Backup)
- [ ] Software
	 - [ ] DMZ Router
		- [ ] OPNsense installation (https://docs.opnsense.org/setup.html)
		- [ ] Wireguard Client setup
	- [ ] Router
		- [ ] OpenWRT reinstallation
	- [ ] Switch
	- [ ] Proxy
		- [ ] Debian Server installation (ISO: https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/debian-12.8.0-amd64-DVD-1.iso)
		- [ ] Wireguard Server setup
		- [ ] CrowdSec (https://docs.crowdsec.net/u/getting_started/installation/linux)
	- [ ] MGMT
		- [ ] Debian Server installation (ISO: https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/debian-12.8.0-amd64-DVD-1.iso)
	- [ ] NAS (https://www.truenas.com/download-truenas-scale/)
		- [ ] TrueNAS Scale Installation (https://www.truenas.com/docs/scale/)
			- [ ] Mirrored Boot Drive/Pool (https://www.truenas.com/docs/core/coretutorials/systemconfiguration/mirroringthebootpool/)
			- [ ] Storage Pool with ZFS RAID-Z2 (4x4TB Disks, for $\leq 2$ Drive Failures) (https://www.truenas.com/docs/scale/scaletutorials/storage/createpoolwizard/)
	- [ ] Game Server
		- [ ] Debian Server installation (ISO: https://cdimage.debian.org/debian-cd/current/amd64/iso-dvd/debian-12.8.0-amd64-DVD-1.iso)
		- [ ] CubeCoders AMP installation (https://cubecoders.com/AMP/Install)
	- [ ] working Backups (https://restic.net/)
		- [ ] DMZ (FreeBSD) -> NAS (FreeBSD)
		- [ ] Switch -> NAS (FreeBSD)
		- [ ] Router -> NAS (FreeBSD)
		- [ ] MGMT (Debian) -> NAS (FreeBSD)
		- [ ] Gameserver (Debian) -> NAS (FreeBSD)
		- [ ] PC (Windows 11) -> NAS (FreeBSD)
		- [ ] Laptop (Arch) -> NAS (FreeBSD)
		- [ ] NAS (FreeBSD) -> ??
- [ ] Network
	- [ ] DMZ Router
	- [ ] Router
	- [ ] Switch
	- [ ] Proxy

## Deprecated?
- [ ] Fix Network
	- [ ] fix Networking/Routing problem with Wireguard and Forwarding
		- might be local NAT/Proxy config
		- accessing gamingandfriends.com/test (VM: 10.0.30.160?) from internet works, but f.e. updating same VM through same route not working (cant access server)
	- [ ] Wireguard
		- [ ] fix Wireguard Interface shutting down from time to time
		- [ ] auto update Wireguard Peers (if IP changes)
			```c
			if (!peer_connection) {
				server.remove_peer()
				server.connect_to_server()
				server.test_connection()
				client.test_connection()
			}
			```
