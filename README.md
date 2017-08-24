# OSSN Installer
An installer script for Open Source Social Network

## Information
This script will install all of the required programs, services, and dependencies needed to run OSSN. I wrote this after reading so many people were struggling with the installation process, namely permissions and configuring Apache. This script serves as an easy install point to get anyone up and running.

It should be stated that this script has only been tested on a fresh installation of Ubuntu 16.04, but will work on later versions as well. Do not use if you're running multiple Apache virtual hosts on the same server. This script will break it upon reconfiguring the 000-default.conf for OSSN.

## How to use

### Clone this repository
`git clone https://github.com/themattbook/ossninstaller.git`

#### Change into the directory
`cd ossninstaller`

#### Make installer script executable
`chmod +x ./ossn_installer_ubuntu.sh`

#### Install OSSN
`sudo ./ossn_installer_ubuntu.sh`
