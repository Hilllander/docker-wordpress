# docker-wordpress

This will pulling and create Wordpress, MySQL, phpMyAdmin containers into Docker Desktop by using docker-compose script.

How to install Wordpress on Docker using docker-compose.

# Install Docker Desktop
1. Download and install Docker Desktop from https://docs.docker.com/docker-for-windows/install/
2. For Windows 10 Pro/Enterprise, enable Windows Linux Subsystems (WSL) v2 to allow Linux kernel can be run on Windows OS.
3. When finish, start Docker Desktop and open Windows PowerShell with Administrator permission.
4. Try to pull image and deploy test container with below command:
      docker run hello-world
5. If the message "Hello World!" appear on you PowerShell screen, you are now good to go.

# Install Git
1. Download and install Git with its components (Git Bash, Git GUI) from https://git-scm.com/downloads

# Install Wordpress on Docker
1. In PowerShell screen, go to other drive/directory which you need to shared between Windows host and Linux container.
   for example:   cd d:\dockershared
2. Create your local directory in this directory e.g. mkdir wpsources
3. 
