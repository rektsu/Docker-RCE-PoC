# Docker-RCE-PoC
RCE PoC for Docker

# Short Description
This is a PoC of an RCE from docker container to host machine.

# Conditions
Abusing cgroups and linux capabilities.
Notify_on_release value has to be set to 1 for this to work.
Terminate all processes so notify_on_release can launch the commands stored in the host machine.
