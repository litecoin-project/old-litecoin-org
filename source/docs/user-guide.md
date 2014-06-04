---
layout: layout
lang: en
id: end-user-guide
title: "End-User Guide - Bitcoin"
---

[transaction malleability]: #term-transaction-malleability

# End-User Guide

<div markdown="1" id="toc" class="toc"><div markdown="1">

* Table of contents
{:toc}

</div></div>


<!--#md#<div markdown="1" class="toccontent">#md#-->


## Viewing Hidden Files/Folders

### Windows 7

### Windows 8

### Linux
1. Navigate to the directory/folder you would like to display the contents of.
2. Use the command 'ls -al' to list all files or folders, including hidden ones.  
```
[username@localhost ~]$ cd .bitcoin/  
[username@localhost .bitcoin]$ ls  
[username@localhost ~]$ ls  
Documents    Pictures    Videos    Downloads  Music    Desktop                 
[username@localhost ~]$ ls -al  
total 288  
drwx--x--x. 44 username username  4096 Apr 18 10:23 .  
drwxr-xr-x.  7 root      root       4096 Apr 13 11:35 ..  
-rw-------.  1 username username 12937 Apr 18 10:22 .bash_history  
-rw-r--r--.  1 username username    18 Aug  9  2013 .bash_logout  
-rw-r--r--.  1 username username   193 Feb 15 17:16 .bash_profile   
-rw-r--r--.  1 username username   291 Feb 15 17:19 .bashrc  
drwxrwxr-x.  4 username username  4096 Apr  4 15:14 bin  
drwxrwxr-x.  5 username username  4096 Mar 21 15:06 .bitcoin  
drwxr-xr-x.  2 username username  4096 Mar 25 16:59 Desktop  
drwxr-xr-x.  3 username username  4096 Mar 25 17:12 Documents  
drwxr-xr-x.  7 username username  4096 Apr 16 12:04 Downloads  
drwxr-xr-x.  2 username username  4096 Jan 20 18:02 Music  
drwxr-xr-x.  6 username username  4096 Apr 13 13:07 Pictures  
drwxr-xr-x.  2 username username  4096 Mar 26 08:27 .vim  
-rw-------.  1 username username  7362 Apr 13 14:17 .viminfo  
```

### Mac OSX


## Viewing File Extensions

### Windows 7
1. Open Windows Explorer.
2. If you do not see a menu bar ("File", "Edit", "View", etc), press the 'alt' button.  
![file-ext-win7-1](/images/end-user/file-extensions-win7/alt-menu-bar.png)  

3. Click on 'Tools' -> 'Folder Options'.  
![file-ext-win7-1](/images/end-user/file-extensions-win7/tools.png)  

4. You should now see the popup 'Folder Options' window.  
![file-ext-win7-1](/images/end-user/file-extensions-win7/folder-options.png)  

5. Click on the 'View' tab.  
6. Uncheck 'Hide extensions for known file types.'  
7. Click the 'Apply' button, then 'OK' button.  
![file-ext-win7-1](/images/end-user/file-extensions-win7/view-settings.png)  

### Windows 8  
1. Open Windows Explorer.  
2. Click the 'View' tab.   
![file-ext-win7-1](/images/end-user/file-extensions-win8/view.png)  

3. Click on 'Options' -> 'Change folder and search options'  
![file-ext-win7-1](/images/end-user/file-extensions-win8/options.png)  

4. You should now see the popup 'Folder Options' window.  
5. Click the 'View' tab.   
![file-ext-win7-1](/images/end-user/file-extensions-win8/folder-options.png)  

6. Uncheck 'Hide extensions for known file types.'  
7. Click the 'Apply' button, then 'OK' button.    
![file-ext-win7-1](/images/end-user/file-extensions-win8/unhide-extensions.png)  


### Linux
On linux systems, extensions are usually not hidden to begin with.

1. Navigate to the directory/folder you would like to display the contents of.
2. Use the command 'ls' to list all files or folders.  This will list them with their file extensions as well.

{% highlight bash lineos %}
[username@localhost ~]$ cd .bitcoin/
[username@localhost .bitcoin]$ ls
bitcoin.conf  blocks  chainstate  __db.001  __db.002  
__db.003  db.log  debug.log  peers.dat  testnet3  wallet.dat
{% endhighlight %}


### Mac OSX
On Mac systems, extensions are usually not hidden to begin with.  
![file-ext-osx](/images/end-user/file-extensions-osx/ushow-file-ext.png)    


## Finding the Data Directory 

### Bitcoin-qt  

#### Windows 8
1. Open the run window by pressing 'Windows' + r.
2. Type in '%APPDATA%'.  
![file-ext-win7-1](/images/end-user/bitcoin-qt-win8/run-window.png)

3. Once you hit enter or press 'OK', you should see the following Appdata Roaming window.  
4. Open the 'Bitcoin' directory.  
![file-ext-win7-1](/images/end-user/bitcoin-qt-win8/appdata.png)

5.  This is where you will find all the data that is held by your wallet.  
![file-ext-win7-1](/images/end-user/bitcoin-qt-win8/bitcoin.png)

6.  The only important file you need to backup and keep secure, is the wallet.dat file as shown below.  (If you cannot see the .dat extention, refer to the __[file extension][view-file-extentions]__ section)  
![file-ext-win7-1](/images/end-user/bitcoin-qt-win8/wallet.png)

#### Windows 7
1. Open the run window by:
 1. 'Windows' + r   OR
 2.  click the start button and type in 'run' into the search bar.

#### Linux

#### Mac OSX

### Electrum

#### Windows 8
1. Open the run window by pressing 'Windows' + r.
2. Type in '%APPDATA%'.  
![file-ext-win7-1](/images/end-user/electrum-win8/run-window.png)

3. Once you hit enter or press 'OK', you should see the following Appdata Roaming window.  
4. Open the 'Electrum' directory.  
![file-ext-win7-1](/images/end-user/electrum-win8/appdata-window.png)

5.  This is where you will find all the data that is held by your wallet.  
![file-ext-win7-1](/images/end-user/electrum-win8/electrum-window.png)

6.  The only important file you need to backup and keep secure, is the default_wallet file as shown below.  
![file-ext-win7-1](/images/end-user/electrum-win8/wallet.png)

#### Windows 7
1. Open the run window by:
 1. 'Windows' + r   OR
 2.  click the start button and type in 'run' into the search bar.

#### Linux

#### Mac OSX

##Checking GPG Signature

###Windows 7
*This step-by-step guide was provided by [lavajumper](https://litecointalk.org/index.php?action=profile;u=11329) on litecointalk.org forum.  Check the orignal post [here](https://litecointalk.org/index.php/topic,5116.0.html).  

1. Download gpg4win:  
	http://www.gpg4win.org/download.html  
	Get the full version, its the first link.  

2. Run the installer.   
	Choose where you want it. When you get to this screen, check the box and move on.  
	![](/images/end-user/gpg4win/gpg4win_1.png)   

3. Create a certificate for yourself:  
	Start Kleopatra.  
	Now, generate a new certificate for yourself.  
	![](/img/end-user/gpg4win/gpg4win_2.png)  
	![](/img/end-user/gpg4win/gpg4win_3.png)  
	![](/img/end-user/gpg4win/gpg4win_4.png)  

4. Click on 'Advanced Settings'  
	Make it usable for Signing, Encryption, Authentication.  
	I generally make a self cert, that is not going 'into the wild' usable for a long time.    
	![](/images/end-user/gpg4win/gpg4win_5.png)  


5. Create a password.  
	It will ask for a password. Give it one. Make it good, but NEVER lose it.  
	![](/images/end-user/gpg4win/gpg4win_6.png)  

6. Click 'Finish'  
	![](/images/end-user/gpg4win/gpg4win_7.png)  

7. Set up the Directory Service:  
	Now, go to Settings| Configure Kleopatra  
	Click 'New' to set up a directory server.   
	Scheme is 'hkp', Server name is 'pgp.mit.edu', port 11371  
	![](/images/end-user/gpg4win/gpg4win_8.png)  

8. Search/Import LiteCoinDev's certificate  
	Click 'Ok' and then 'Lookup Certificates on Server'  
	Search for '0xC37E4723969276F5'  

	If you are running a Mac, the builds are signed separately by the Mac developer:  
	http://pgp.mit.edu:11371/pks/lookup?op=vindex&search=0x657EB016521670C0    
	This is because the Dev Team can't do deterministic builds like Linux and Win32.   

9. Select 'Litecoin Dev Team' and 'Import'   
	![](/images/end-user/gpg4win/gpg4win_9.png)  

10. Certify LiteCoinDev's certificate via your cert and LiteCoinDev's fingerprint.  
Click on the Others tab  
Select and right click on Litecoin Dev Team's certificate and chose 'Certify Certificate'  
	![](/images/end-user/gpg4win/gpg4win_10.png)  

11. Certify the new ID, making sure the fingerprint is as below:  
DC38 0DA4 3082 F163 78C9  7414 C37E 4723 9692 76F5  
	![](/images/end-user/gpg4win/gpg4win_11.png)  


If the fingerprint does NOT match...STOP! Bad things are happening. Otherwise, continue.  

12. Select the certificate you created above:  
	![](/images/end-user/gpg4win/gpg4win_12.png)  

13. Verify Litecoin.exe  
Go to File|Decrypt/verify, then select the exe or the corresponding signature   
	![](/images/end-user/gpg4win/gpg4win_13.png)  

14. Click 'Decrypt/Verify'  
	![](/images/end-user/gpg4win/gpg4win_14.png)  


Success!  
	![](/images/end-user/gpg4win/gpg4win_15.png)  



If it fails, STOP. Bad things are happening. Do NOT install that program! Otherwise,

15. Install Litecoin:
Run the Litecoin installer and smile, while enjoying your sense of accomplishment.


###Linux


<!-- Links to terms used in this document (case-insensitive alphabetic order)
---- * Link text is case insensitive in markdown so [Block Chain] and
----   [block chain] are equivalent
---- * If nothing uses one of the below reference links, the reference
----   link must be commented out or it will appear in the rendered page
-->
[view-file-extentions]: #viewing-file-extensions

<script>updateToc();</script>



