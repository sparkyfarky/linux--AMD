# linux--AMD
linux- AMD GPX n ess git res
1. Download the drivers from AMD's website that correspond with your version of Ubuntu. 

2. Run "sudo apt-get update" 

3. Run "sudo apt-get dist-upgrade" 

4. Install the dependencies by running " sudo apt-get install linux-headers-generic build-essential cdbs fakeroot dh-make debhelper debconf libstdc++6 dkms libqtgui4 wget execstack libelfg0 dh-modaliases" 

5. Change the directory to the 'Downloads directory (or the directory where the .run is currently located.) 

6. Make the .run file executable by either clicking "allow file to execute as a program" in the permissions tab under properties or running "chmod +x (AMD Driver .run file)" 

7. Execute the .run file with "./(AMD driver .run file)" 

8. Select 'generate a distribution specific package' 

9. Select the package for your distribution. 13.10 is 'Ubuntu/saucy' 13.04 is 'Ubuntu/raring' and 12.04.02 or 12.04.03 is "Ubuntu/precise' 

10. Install the .deb packages using "sudo dpkg -i *.deb" 10.5 If any dependencies are not installed then run "sudo apt-get install -f" 

11. DO NOT REBOOT THE COMPUTER! Run "aticonfig --initial" if you have a single device or "aticonfig --adapter=all --initial" if you are running multiple graphics adapters eg. crossfire. 

12. Now you can reboot the computer. 

13. The linux version of the catalyst control center is like that guy you are pretty sure sells drugs on the side. It doesn't work that well. When you try to launch it in administrative mode it works on occasion. Others it just says 'authentication failure' the fail-safe way to do this launch it from the terminal using "sudo amdcccle" or for more experienced linux users, make your own launcher. 

14. Configure the catalyst control center how you please then reboot. It should be ready to use. 

From <https://www.youtube.com/watch?v=mj0oND69is0> 

Uninstalling Programs with Terminal

From <https://www.wikihow.com/Uninstall-Ubuntu-Software#Uninstalling-Programs-with-Ubuntu-Software> 


Look for app


dpkg --list

Update database apps/programs

Sudo dpkg --configure -a


sudo apt-get --purge remove program




From <https://www.wikihow.com/Uninstall-Ubuntu-Software#Uninstalling-Programs-with-Ubuntu-Software> 




