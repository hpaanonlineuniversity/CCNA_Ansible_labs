
# install ansible at eve-ng server with the following command

sudo apt install python3-paramiko sshpass ansible



# Ping all devices
ansible all -m ios_ping -a "dest=x.x.x.x"

# Show clock on all devices
ansible all -m cisco.ios.ios_command -a "commands='show clock'"

# Save configuration on routers
ansible routers -m cisco.ios.ios_command -a "commands='write memory'"

# Show interfaces on switches
ansible switches -m cisco.ios.ios_command -a "commands='show interfaces status'"

