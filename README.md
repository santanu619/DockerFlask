# DockerFlask Installation
## System Requirements:-
Our Windows machine must meet the following requirements to successfully install Docker Desktop.
### WSL 2 backend
* Windows 10 64-bit: Home or Pro 2004 (build 19041) or higher, or Enterprise or Education 1909 (build 18363) or higher.
* Enable the WSL 2 feature on Windows. For detailed instructions, refer to the Microsoft documentation.
* The following hardware prerequisites are required to successfully run WSL 2 on Windows 10:
    * 64-bit processor with Second Level Address Translation (SLAT)
    * 4GB system RAM
    * BIOS-level hardware virtualization support must be enabled in the BIOS settings. 
* Download and install the Linux kernel update package.
## What’s included in the installer
The Docker Desktop installation includes Docker Engine, Docker CLI client, Docker Compose, Docker Content Trust, Kubernetes, and Credential Helper.
Containers and images created with Docker Desktop are shared between all user accounts on machines where it is installed. This is because all Windows accounts use the same VM to build and run containers. Note that it is not possible to share containers and images between user accounts when using the Docker Desktop WSL 2 backend.
Nested virtualization scenarios, such as running Docker Desktop on a VMWare or Parallels instance might work, but there are no guarantees.
## About Windows containers
* Switch between Windows and Linux containers describes how we can toggle between Linux and Windows containers in Docker Desktop.
* Getting Started with Windows Containers (Lab) provides a tutorial on how to set up and run Windows containers on Windows 10, Windows Server 2016 and Windows Server 2019. It shows us how to use a MusicStore application with Windows containers.
## Install Docker Desktop on Windows
1. Double-click Docker Desktop Installer.exe to run the installer.
**If you haven’t already downloaded the installer (Docker Desktop Installer.exe), you can get it from Docker Hub. It typically downloads to your Downloads folder, or you can run it from the recent downloads bar at the bottom of your web browser.**
2. When prompted, ensure the Enable Hyper-V Windows Features or the Install required Windows components for WSL 2 option is selected on the Configuration page.
3. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.
4. When the installation is successful, click Close to complete the installation process.
5. If your admin account is different to your user account, you must add the user to the docker-users group. Run Computer Management as an administrator and navigate to Local Users and Groups > Groups > docker-users. Right-click to add the user to the group. Log out and log back in for the changes to take effect.


