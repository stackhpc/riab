# The upstream image includes the Ansible plugin but no
# Ansible command, so let's fix that in another layer.
FROM rundeck/rundeck:3.0.6

RUN sudo apt-get update && sudo apt-get install -y ansible \
	&& sudo rm -rf /var/lib/apt/lists/*
