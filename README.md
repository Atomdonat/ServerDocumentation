# ServerDocumentation
## To-Do:
- [ ] Hardware
- [ ] Software
	 - [ ] DMZ Router
		- [ ] OPNsense installation (https://docs.opnsense.org/setup.html)
		- [ ] Wireguard Client setup
	- [ ] Router
		- [ ] OpenWRT reinstallation
	- [ ] Switch
	- [ ] TrueNAS
	- [ ] Game Server 
		- [ ] CubeCoders AMP installation (https://cubecoders.com/AMP/Install)

- [ ] Network
	

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
