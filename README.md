# Docker-RCE-PoC
RCE PoC for Docker

# Short Description
This is a PoC of an RCE from docker container to host machine.

# Conditions
Abusing cgroups, linux capabilities and AppArmor misconfigurations.
Notify_on_release value has to be set to 1 for this to work.
Terminate all processes so notify_on_release can launch the commands stored in release_agent

# Running the RCE
download the exploit.sh file and modify the $var value to execute the command you wish in the host machine. I.E ls, id, pwd, etc...
cat /output to see the output of the command ran.

# Case of Use
use exploit.sh to list users and grab possible .ssh authorized_keys to connect to the host machine through ssh service if available, list networks of the organization, users, services installed, etc.
