# Customize Xfce Desktop
*Automate the customization of your Xfce Desktop to Look Like macOS Big Sur*
#
## Prerequisite:
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

* Logout and login again after the execution finishes
