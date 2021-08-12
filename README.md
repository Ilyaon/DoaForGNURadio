# DoaForGNURadio 12/08/21
We will be using the excellent https://github.com/MarcinWachowiak/GNU-Radio-USRP-Beamforming repository and setting it up in the current versions of the programs needed.  
This is a step by step guide from the basic ubuntu installation, we will need (*this guide is for linux ubuntu*):  
1) [ ] gnu radio version 3.8 (older)
2) [ ] install MarcinWachowiak's repository for application of direction/angle of arrival estimation.
3) [ ] make sure we have the needed libraries.

# Downloading 3.8 version of GNU Radio
![image](https://user-images.githubusercontent.com/88839484/129210066-d1d681f9-b5d5-48f0-99b2-61edc0fc1cd5.png)  
At: https://wiki.gnuradio.org/index.php/InstallingGR#For_GNU_Radio_3.8_or_Earlier
First, we will need to follow these steps in order to get the 3.8 version of GNU Radio.  
Any other approach did NOT work for me personally.   
This step will take awhile so be prepared.   
**At this step** ![image](https://user-images.githubusercontent.com/88839484/129210762-813e9fb6-369d-4655-9797-24e78d73997a.png)  
instead type: `pip3 install git+https://github.com/pyqtgraph/pyqtgraph  `

# Installing Marcin Wachowiak's DOA/AOA repository
Second, We will install the repository: https://github.com/MarcinWachowiak/GNU-Radio-USRP-Beamforming
![image](https://user-images.githubusercontent.com/88839484/129212382-9ecd5662-3326-4a7d-a42b-071073736f23.png)  
**After this step** ![image](https://user-images.githubusercontent.com/88839484/129213128-abe3eb5d-41ed-45a9-ad36-ae2f7551b0f5.png)  
Add these lines of code to update the problematic addons:  
```
cd 
dpkg -l | grep -i eigen3    
sudo apt-get install libeigen3-dev    
sudo apt update
sudo apt install swig
```
Then continue the process from where you left off.
# Reboot your ubuntu and congratulations.
You can try and run one of the simulations that are located in the *GNU-Radio-USRP-Beamforming* folder in your file manager
