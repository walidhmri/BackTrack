# A Guide to Backtrack 5 R3 Linux Commands 
Prepared by: Ameer Sameer Hamood University of Babylon - Iraq Information Technology - Information Networks \ Edited by : Oualid Hamri
![image](https://user-images.githubusercontent.com/94682505/166089277-6095c862-a38d-4cbf-8083-2e20b4a8e92d.png)
# Backtrack 5 R3 : 
is one of the Linux operating system so we can operate Backtrack  with  Linux  common  command.  Learning  Linux  operating system is very easy and you must familiar with the unix commands if you want  use  Backtrack  5  R3.  Here  I  am  post  some  common  Linux commands which will be used on Backtrack 5
# Logging in to BackTrack
Once  the installation  of  BackTrack is  done, the  default username  and password required to log in are root / toor.  
NOTE: You will not be able to see the password as you type it.
# Starting a GUI Environment 
After you are logged in you can start the GUI Environment by issuing the startx command.
# X wont start!
In rare occasions (such as after a VMware tools install, or when using unsupported Video cards), X will refuse to start. If that happens you have several options you can try in order to fix the issue:

 Reconfiguring the X server package, you can reset (and often fix) Xorg configurations with the following command:
```bash
root@bt:~# dpkg-reconfigure xserver-xorg
```
 If you are using Backtrack 5 on x64 with KDE you should try the following: 
```bash
root@bt:~# rm /root/.kde/cache-*
```
NOTE: Sometimes you may need to also remove the cache folders in /var/tmp by issuing the following command: 
```bash
root@bt:~# rm -rf /var/tmp/kdecache-*
```
