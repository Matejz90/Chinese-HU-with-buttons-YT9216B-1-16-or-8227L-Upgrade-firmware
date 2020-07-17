# Story  
Because of one week searching like idiot on internet, mostly on Russian sites i can now read Cyrilic and speak something (Nazdrovje!!!) i found way how to update Chinese crap HU to little bit more decent software with ROOT, TWRP, and better radio app with RDS.  
  
#### If you have HU (head unit) with phisical buttons and USB socket on front then this tutorial is for you because you have similar crap like i have.  
  
#### What was symptoms of not working flash procedure? 
- USB flash with XYAUTOUPG folder - hell yeah haha (no go) 
- flash with SP_Flash_Tool - are you insane? (no go)
- trying boot with pressed buttons - why will you do that?
- connecting to pc - not even bing bing sound when you connect something
- when you reset HU connected to PC you get USB not recognized popup and in device manager no id or description for device 
- and other nasty stuff...  
  
#### Conclusion:  
Because back 4 pin port is connected to front USB socket, something interfer connection and cannot be flashed ordinary way. Not even with 6 pin port on back.  
#### Solution: 
Dissasembly back plate and disconnect ribbon cable from front USB socket to motherboard and flash in ordinary way  

# Prerequisites:  
1.) Screwdriver  
2.) HU with phisical buttons on front and USB socket, model 8227L or YT9216B with 1GB ram and 16GB rom. Mine has come with YT9216B_00002_V_004_20190826 version, Android 8.1 Go (chinese scam because it isn't 8.1) and MCU 3.1  
3.) You need to make male-male USB cable (or buy it). You can take two old cables, cut booth and solder or tangle wires together. Take care of color matching (Black-black, White-white etc.)  
4.) Download zip from [4pda](https://4pda.ru/forum/index.php?showtopic=936535&st=14340#entry89982813) with name (direct link to gdrive): [YT9218_00002_V004_20190912 (UI1) ROOT , TRPW](https://4pda.ru/pages/go/?u=https%3A%2F%2Fdrive.google.com%2Fopen%3Fid%3D1eooFBvIp-W-OnpAq6WPuqgG6cDhd2FGv&e=89982813&f=https%3A%2F%2F4pda.ru%2Fforum%2Findex.php%3Fshowtopic%3D936535%26st%3D14340%23entry89982813) from user [Maxkir](https://4pda.ru/forum/index.php?showuser=8537307) (tnx dude)  
5.) Download [SP_Flash_Tool_v5.1924_Win](https://spflashtools.com/windows/sp-flash-tool-v5-1924)  
6.) Download [SP_Driver_v2.0](https://androidfilehost.com/?fid=24438995911977169)  
7.) Windows 10 x64 PC  
8.) PSU (12v, 1A is enough)  
9.) Knife (sharp if you have)  

# OK lets go!  
1.) First reboot PC to driver signature disable mode. Go to start, click shift + windows key on keyboard, and click power - restart. Go to troubleshoot - advanced options - startup settings - restart. When PC reboots hit F7 button  
2.) Then extract SP_Driver_v2.0 from zip and install driverinstall.exe with admin rights (right click - run as administrator). You need few times click allow when installing drivers (or something in box with x)  
3.) Extract YT9218_00002_V004_20190912  
4.) Extract SP_Flash_Tool_v5.1924_Win and run like administrator. In Download Agent field link MTK_AllInOne_DA.bin and in Scatter-loading file link from extracted YT9218_00002_V004_20190912 MT3367_Android_scatter.txt. Deselect preloader if is selected!!!!!  
5.) Take apart your HU. Unscrew 4 screws on back plate. Then you will see one ribbon cable (flat cable) that goes from LCD site where is USB socket to motherboard. On motherboard disconnect this cable.  
6.) If you have 4 pin USB cable then connect this cable in back of HU in 4 pin port. If you have only 6 pin cable then try to modify connector on cable and cut away two empty "pins" and connect cable to 4 pin HU port  
7.) In SP_Flash_Tool_v5.1924_Win hit Download button  
8.) Connect male-male USB cable with cable in step 6.  
9.) Voila. Your PC start flashing stupid HU. Wait few minutes till SP_Flash_Tool_v5.1924_Win show new popup with flash successfull image. Disconnect cables and reboot HU with disconnecting PSU. Reconnect power and wait till HU load all stuff and boot to loader.  
<p align="center">
  <img width="460" height="300" src="https://github.com/Matejz90/Chinese-HU-with-buttons-YT9216B-1-16-or-8227L-Upgrade-firmware/blob/master/Pictures/110167055_284396332837423_7813481836340363955_n.jpg?raw=true">  
</p>  
10.) Change language from Russian to whatever you want.  
11.) Go to Car Settings - Factory Settings (PIN: 8888) - Color Setting and scroll to bottom and change slider AVDD to 2. With this you will eliminate screen flickering.   
<p align="center"><img width="460" height="300" src="https://github.com/Matejz90/Chinese-HU-with-buttons-YT9216B-1-16-or-8227L-Upgrade-firmware/blob/master/Pictures/110167055_284396332837423_7813481836340363955_n.jpg?raw=true"></p>  
12.) Go to Play Store, login, and update all apps.  
  
# Addons  
Now you can change Radio apps if you don't like existing (in this version contain app with RDS), launcher, etc...If you want to change files in download Root Explorer Classic and use it  
  
There you have launchers (you can install all of thems and use whitch you want. You can save favorite with alway use when HU reboots): https://4pda.ru/forum/index.php?act=findpost&pid=80952587&anchor=Spoil-80952587-13 
<p align="center"><img width="460" height="300" src="https://github.com/Matejz90/Chinese-HU-with-buttons-YT9216B-1-16-or-8227L-Upgrade-firmware/blob/master/Pictures/17417269.jpg?raw=true"></p>
<p align="center">
pic from 4PDA
</p>
