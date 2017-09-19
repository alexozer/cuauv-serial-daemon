# Serial notes

## Notes
- Devices are silent in disconnected state to force hosts to reconnect

## Questions

### General
- Why aren't registers abstracted by the devices / API?

### Heartbeat
- Why do heartbeat packets contain softkill / hardkill flags?
- Why not have *kill packets as separate packets, as heartbeats will kill connection if idle anyway
- Maybe all packets should count as "heartbeat", and periodic heartbeat packets are just "null"

### Packet validation
- Is t_byte higher than what the baud rate would account for? What exactly is it?
- How do hosts and devices know the expected length of packets (based on type and payload)?
	- Is the size (payload) constant for a given packet type?
	- Does it matter?


