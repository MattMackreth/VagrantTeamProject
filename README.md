# How to install developer environment
If you already have vagrant and virtualbox (and they are working correctly) skip to step 7
## 1. Install Vagrant
Download and install the most up to date version of vagrant by Hashicorp.
Available at https://www.vagrantup.com/downloads.html

## 2. Install VirtualBox
Download and install VirtualBox 6.0 by oracle.
Available at https://www.virtualbox.org/wiki/Downloads
As well as the Extension Pack from the same page.

## 3. Ensure you have virtualization turned on in BIOS
Turn off your machine. Then turn it back on while holding F10. Navigate to System Configuration and ensure virtualization technology is enabled. Then exit while saving changes.

## 4. Ensure HyperV is turned off.
Search for and go into 'Turn Windows Features on or off' and ensure the HyperV box is unchecked. If it was checked, uncheck it and restart your computer.

## 5. Enable VirtualBox Host network
 1. Go to control panel
 2. Go to network and internet
 3. Go to network and sharing centre
 4. Go to change adapter settings.
 5. Right click on VirtualBox Host Only Network (or Ethernet 2) and click on properties.
 6. Click install
 7. Click Services
 8. Click add
 9. On the left under Manufacturer click Oracle Corporation.
 10. Press OK on all dialogue boxes.

## 6. Start Oracle VirtualBox Manager
Type in $ sc start vboxdrv

## 7. Pull all files down into your directory.
Using $ git pull

## 8. Make sure you have the vagrant hostsupdater plugin
Type in $ vagrant plugin install vagrant-hostsupdater

## 9. Spin up the virtual machine
Type in $ vagrant up

## 10. Enter the virtual machine
Type in $ vagrant ssh
You are now logged into the virtual machine

## 11. Ensure everything is up to date
Type in $ sudo apt-get update

## 12. Start NGINX server
Type in $ sudo apt-get install nginx -y

## 13. Start up NGINX
Type in $ sudo systemctl start nginx

## 14. You can now access the server
Going to http://development.local will show you the default NGINX welcome page.
\n
:pray:S:pray:E:pray:L:pray:F:pray:5:pray:
