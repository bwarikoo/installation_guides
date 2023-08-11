Steps to install Docker on an Ubuntu machine.

1. ```sudo apt-get update```
2. ```sudo apt install docker.io```

After installing docker, it is important to add the "ubuntu" or the current user to the "docker" group in order to execute docker commands on the instance. Run the below command to modify the "docker" group to add the current user of the system i.e., ubuntu. 

```sudo usermod -aG docker $USER```
Here, $USER represents the current user.

After running the usermod command, reboot your Ubuntu instance for the group changes to reflect. You can reboot your instance by executing below command.

```sudo reboot```

If you are going to use docker-compose in your projects, you need to install "docker-compose" separately using below command. 

```sudo apt install docker-compose```
