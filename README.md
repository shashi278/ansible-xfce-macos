# Xfce to Macos
*Automate the customization of your Xfce Desktop to Look Like macOS Big Sur*
#
**Automated all steps shown in this video by LinuxScoop: https://youtu.be/uvvoJU69uNo**
## Prerequisite:
* You're on Ubuntu
*	**Install Dependencies**
	```
	sudo apt update
	sudo apt install software-properties-common
	sudo add-apt-repository --yes --update ppa:ansible/ansible
	sudo apt install ansible git xfce4
	```
*	**Switch to xfce-session**
	* Logout
	* On the login screen, click on the settings icon in the bottom-right corner and select xfce-session
	* Login

## Automate and chill
* Open terminal and paste below command
	```
	ansible-pull -d ~/Documents/modify-desktop-ansible -U https://github.com/shashi278/xfce-to-macos.git ~/Documents/modify-desktop-ansible/playbook/setup.yml -K
	```

* Enter password when prompted for `BECOME password`

* Chill

* Logout and login again after the playbook execution finishes

* You can always go back to you Ubuntu by logging out from xfce.

## Result
![demo.gif](https://raw.githubusercontent.com/shashi278/xfce-to-macos/main/result/demo.gif)


### Note:
It's advisable to always verify the source code of an automation script before executing them on your machines.
