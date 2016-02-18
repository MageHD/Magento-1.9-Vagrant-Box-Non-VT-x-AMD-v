# Magento-1.9-32-Bit-Vagrant-Box-Non-VT-x-AMD-v
It just Works!!

This repo will allow you to run a vagrant box for local Magento development. This was developed to fix the issue with development on computers without virtualization technology (VT-x/AMD-v). When the script is complete, you will have a fully functional Vanilla Magento install for local development.  
#Needed: 
1. Vagrant
2. Virtualbox
3. Git for Windows (Allows for running Linux commands)
4. Vagrant Host updater <a href="https://github.com/cogitatio/vagrant-hostsupdater">Vagrant Host Updater</a>

#Steps 
1. Install Virtualbox, Vagrant, & Git for Windows
2. Register the Virtualbox included in the repo
3. Create a project folder 
4. Right click within the folder and Launch Git Bash 
5. Using Git Bash clone the repository within your project folder using "." as the folder location 
6. Edit the vagrant file and add your hostname(local.testdomain.com) and an ip address (IP adress must be unique) 
7. Open toolsprovision.sh and update the baseurl on line 3. (Make a note of the admin login information) 
8. Run "vagrant up" in the project folder

#Important Notes
1. Update the Vagrant file to reflect the domain name you're using
2. Update the toolsprovision.sh file on line 3 (Base url) with the domain you're using
This Repo was brought to you by Gary Pettigrew of <a href="rushmediastudios.com">Rush Media Studios</a>

#What is does
1. Install Magerun Globally
2. Install Modman Globally
3. Install Magento 1.9.2
4. Install Magento sample data

#The Admin
The admin credentials is user: admin pw: password123
