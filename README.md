# docker-wordpress

This will pulling and create Wordpress, MySQL, phpMyAdmin containers into Docker Desktop by using docker-compose script. Please carefully read below step-by-step on how to install Wordpress on Docker using docker-compose.

## Install Docker Desktop
1. Download and install Docker Desktop from https://docs.docker.com/docker-for-windows/install/
2. For Windows 10 Pro/Enterprise, enable Windows Linux Subsystems (WSL) v2 to allow Linux kernel can be run on Windows OS.
3. When finish, start Docker Desktop and make sure that you are running on Linux container mode.
4. Open Windows PowerShell with Administrator privilage (Run As Administrator). Pull image and deploy test container with command:
     `docker run hello-world `
5. If the message "Hello World!" appear on you PowerShell screen, you are now good to go.

## Install Git
Download and install Git with its components (Git Bash, Git GUI) from https://git-scm.com/downloads

## Install Wordpress on Docker
1. In PowerShell screen, go to directory you need to use as home directory, for example: `cd d:\dockershared`
2. Create new home directory in above directory by `mkdir wpsources` and enter to this by `cd wpsources`
3. Clone docker-wordpress Git repository using Git Bash: `git clone https://github.com/Hilllander/docker-wordpress.git`
4. Enter `dir` command to view content in "**wpsources**". There are a new directory "**docker-wordpress**" appeared. 
5. Enter `cd docker-wordpress`, check content in **docker-wordpress** directory, there should have **docker-compose.yml** configuration file in it.
7. Enter `docker-compose up -d` : to pulling images and create Wordpress, MySQL, phpMyAdmin stacks containers.
8. When done, you can access Wordpress from http://localhost:8800 and PMA from http://localhost:8801 from default port configurations.

Now you are going to next steps of Wordpress installation which I'm not mentioned in this (lots of steps in Youtube:).
