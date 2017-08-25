# OSSN Installer
An installer script for Open Source Social Network

## Introduction
This script will install all of the required programs, services, and dependencies needed to run OSSN. I wrote this after reading so many people were struggling with the installation process, namely permissions and configuring Apache. This script serves as an easy install point to get anyone up and running.

It should be stated that this script has only been tested on a fresh installation of Ubuntu 16.04, but will work on later versions as well. Do not use if you're running multiple Apache virtual hosts on the same server. This script will break it upon reconfiguring the 000-default.conf for OSSN.

That being said, please use a fresh installation of Ubuntu 16.04 and higher before running.

## How to use

#### Step 1: Download the Script
`wget https://raw.githubusercontent.com/themattbook/ossninstaller/unstable/ossn_installer_ubuntu.sh`

#### Step 2: Make installer script executable
`chmod +x ./ossn_installer_ubuntu.sh`

#### Step 3: Install OSSN
`sudo ./ossn_installer_ubuntu.sh`

You will be prompted for MySQL credentials a few times throughout the installation process. Upon completion, navigate your browser to the URL of IP of your server. You should be greeted with an Installation page for OSSN showing that all requirements are in blue, meaning they're satisfied and ready to proceed.

![OSSN Installed](https://github.com/themattbook/ossninstaller/raw/unstable/ossn_install.png)

## Additional Information
#### Future Development
Currently, only Ubuntu 16.04 is supported. I will eventually add additional Linux distros to the project. Each distro will have its own script file.

#### MySQL setup
As the script goes through the installation process, you will be prompted for MySQL credentials and input on how to configure `mysql_secure_installation` and phpmyadmin. For `mysql_secure_installation`, simply answer "N" to the first two prompts and "Y" for the remainder. For phpmyadmin, be sure to select "Apache" and for any other prompts, just press ENTER to set default values.

## Support
While my time is limited and spent on other projects, feel free to report an issue if you encounter any bugs or quirks that you feel aren't expected behavior. Rest assured, improvements will be made over time. For the meantime, this should get a lot of people up and running. Enjoy.
