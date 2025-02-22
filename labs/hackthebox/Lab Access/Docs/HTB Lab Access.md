Hack The Box

Lab

https://help.hackthebox.com/en/articles/5185687-introduction-to-lab-access

Introduction to Lab Access

Learn how to connect to the VPN and access Machines on HTB Labs.

Ryan Gordon avatar
Written by Ryan Gordon
Updated over 11 months ago

Over at Hack The Box, we use OpenVPN connections to create links between you and our labs and machines. You may be familiar with one of the many personal VPN services available to individuals, but our VPN serves an entirely different purpose. 

A personal VPN is a service that encrypts a device's internet connection and routes it through a server in a location of the user's choosing. This can be used to protect the user's privacy, as well as to bypass internet censorship. Personal VPNs are often used by individuals to protect their online activity from being monitored or to mask their physical location. 

In contrast, a VPN provided by a company or organization is typically used to allow individuals to access the company's internal network remotely. This type of VPN establishes a secure connection between a user's device and the company's network, allowing the individual to access internal resources as if they were physically connected to the network.

In the case of various VPN configurations we provide, they allow you to access our internal lab networks over the Internet. These configuration files needed to auto-configure your OpenVPN client are called VPN packs or VPN files. 

These will place you in the same IP subnet as the vulnerable machines, allowing you to contact them (and attack them).

 

You will need:

    A Hack The Box account.

    The latest version of OpenVPN. (pre-installed with Kali Linux and ParrotOS)

    A working internet connection.

Tutorial VPN packs

    Starting Point EU Free Access

    Starting Point US Free Access

Free VPN packs

    EU Lab Free Access

    US Lab Free Access

    AU Lab Free Access

    SG Lab Free Access

If you’ve bought a VIP Subscription, you will be able to see the VIP packs as well. These look the same as the Free VPN packs listed above, with the "Free" part changed to "VIP".

While a Linux environment is not required to connect to the VPN, we strongly recommend you use a Linux VM. If you do not have a Linux VM setup, please see the article below:
 
Installing Parrot Security on a VM
 
VPN Settings Configuration

If you want to view and use the currently available VPN controls, you can do so from any page by clicking on the Connect to HTB button next to your profile picture at the top right of the page you're currently on.

You can select the specific content for which you'd like to configure settings from this menu: Machines, Starting Point, Endgame, Fortresses, Pro Labs, and Seasonal.

 

Once you've chosen the content type you're engaging with, you'll have the opportunity to select your preferred method of connecting, either by utilizing a VPN file or opting for the Pwnbox option.

 
OpenVPN :

To configure the settings for the VPN file, you should first select the VPN Access that corresponds to your subscription level, which can be either Free, VIP, or VIP+. This choice is available within one of the four regions: Europe, United States, Australia, and Singapore. Following that, you can proceed to pick the specific VPN server associated with the chosen VPN Access.

 

You can select either the TCP or UDP protocol based on your network circumstances. If your network experiences significant packet loss or congestion, TCP might be the preferable choice because of its ability to handle such issues through error recovery mechanisms. Conversely, when operating on a robust network, UDP is typically the preferred option.

 

You can now click Download VPN after configuring the settings and start using the file.

 
Pwnbox:

The settings for Pwnbox are identical to those of OpenVPN. Additionally, you'll be required to select a Pwnbox location, which will impact the Pwnbox's latency. It's advisable to opt for a nearby location to minimize latency issues.

 

When you click "Start Pwnbox" it initiates the process of launching your virtual machine. This may take a few moments before you're presented with the choices to either "Open Desktop" for a full-screen experience in a new browser tab or "Terminate" the instance.

 

Furthermore, if you wish to modify your VPN Access or VPN Server settings, you'll notice a new button labeled "Switch Pwnbox Access." You'll need to click this button in order to apply and save these changes to the currently running instance.

 

You can utilize either the Pwnbox or the VPN file connection method, but attempting to use both simultaneously will lead to routing errors that will disrupt your connection.

 
Booting up OpenVPN 

After you click the Download button, your OpenVPN file should be found, by default, in the Downloads folder of your Linux distro. You will be using this file as the configuration for your OpenVPN initialization process.

 

Open up a terminal and navigate to your Downloads folder.

 

Then, boot up the OpenVPN initialization process using your VPN file as the configuration file.

 

Once the Initialization Sequence Completed message appears, you can open a new terminal tab or window and start playing. 

 

Please note that you must keep this terminal window open to keep the OpenVPN process running.

 

In case of any issues, check out the article below to start troubleshooting:

 
T: Connection Troubleshooting

 

Below, you can find an explanation of all the VPN control menus:

 
Access

Under the Access menu, you can select from all the different available labs for the main Machines lineup. This includes both free and VIP servers, the latter now including the much-requested AU VIP, SG Free, and SG VIP servers!

 

As a best practice, select the closest lab to you while also considering your account’s VIP status.

 

VIP servers will, of course, have fewer users on them as there are many more than just the free VPN servers. Fewer members mean less traffic and, more importantly, fewer people trying to attack the same Machines as you.
Server

From the Server menu, you can select the actual VPN server you want to connect to. After this step, you should be able to download your .ovpn connection pack directly and proceed with engaging in attacks over the Machines.

 

We have implemented this method of server selection instead of randomly assigning users to the least populated ones due to several requests for multiple teammates attacking the same Machines on the same VPN server to compete against each other. We hope that this will further improve collaboration between teammates and bring your educational progress to the next level for both you and your team or organization!

 
Download

The button to the right of the Server selection menu is the Download button for your now newly generated .ovpn pack. Once clicked, it will initialize a download for your .ovpn file, which you can use to start up the OpenVPN process on your Linux distro that will allow you to connect to the Machines in our labs.

 
Regenerate

In the case where your .ovpn file might be incorrectly generated due to an error, you can regenerate the file by switching back and forth between the Servers on the lab you’ve selected. This will generate the new .ovpn file, which you can directly download to your OS.

 

If even after regenerating, the .ovpn file is still invalid, our support team would be happy to assist you! 




