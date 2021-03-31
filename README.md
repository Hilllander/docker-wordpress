# docker-wordpress

This will pulling and create Wordpress, MySQL, phpMyAdmin containers into Docker Desktop by using docker-compose script.

How to install Wordpress on Docker using docker-compose.

## Install Docker Desktop
1. Download and install Docker Desktop from https://docs.docker.com/docker-for-windows/install/
2. For Windows 10 Pro/Enterprise, enable Windows Linux Subsystems (WSL) v2 to allow Linux kernel can be run on Windows OS.
3. When finish, start Docker Desktop and open Windows PowerShell with Administrator privilage (Run As Administrator).
4. Try to pull image and deploy test container with below command:
     `docker run hello-world `
5. If the message "Hello World!" appear on you PowerShell screen, you are now good to go.

## Install Git
Download and install Git with its components (Git Bash, Git GUI) from https://git-scm.com/downloads

## Install Wordpress on Docker
1. In PowerShell screen, go to directory you need to use as home directory, for example: `cd d:\dockershared`
2. Create new home directory in above directory by `mkdir wpsources` and enter to this by `cd wpresources`
3. Clone docker-wordpress Git repository using Git Bash: `git clone https://github.com/Hilllander/docker-wordpress.git`
4. Use `dir` command to view content in "**wpresources**" directory. There are a new directory name "**docker-wordpress**" appeared. Enter to this directory by `cd docker-wordpress`
5. Check content in **docker-wordpress** directory, there should have **docker-compose.yml** configuration file in it.
6. Pull images and create Wordpress, MySQL, phpMyAdmin stacks containers using :  `docker-compose up -d`
