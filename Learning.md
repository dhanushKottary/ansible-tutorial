### Setup used for the tutorial
1. Using windows Ubuntu WSL as control node.
2. Created 2 VMs using vagrant+virtualbox which are used as manage nodes.
3. Setup SSH connection to both VMs from control node using private key for passwordless authentication.

### Learning
#### Day 2
1. Created `inventory.ini` file where I added all the manage nodes.  
`inventory.ini` file is heart of ansible as ansible uses this file running automation on the desired servers/VMs.  
You can also group servers/VMs in `inventory.ini`.
2. Learnt `ad hoc` commands.  
`ansible -i inventory.ini -m ping all`  
`ansible -i inventory.ini -m "shell" -a "java --version" <any_value>`  
"<any_value>:  can be all or group name or vagrant@<ip_address>"