# psvimgtools-frontend
This is a GUI Interface For Team Molecule / Yifanlu's PSVIMGTools 
Which is a tool that can be used to decrypt & extract PSVita Backup Files (.psvimg) Providing you knew the AID of the account that created the backup, 

this works on every firmware to this date, including 3.63. and probably all future firmwares

the only problem with yifan's inital release, was it was a command-line only tool and also could be a pain in the ass even to some unexperienced users, so this i decided to make this GUI Frontend which will give you all the functions of psvimgtools + more with a GUI. My frontend is written in Python2.7 and supports win32, win64 and linux64 for linux you require libgcrypt11-dev to be installed (sudo apt-get install libgcrypt11-dev) also for everyone, qcma is required for this app to even run.

To design the GUI's i used a tool called PAGE.

Heres a list of features i currently have: 

1. QCMA Intergration. i have tried my best to make this intergrate well with QCMA. For example when you start the app for the first time it will automatically find your QCMA Backups Folder, and will Automatically find your accounts AID, and download CMA Key You can also trigger both of these process'es to occur manually.

2. Quick Resign, Quickly Change the owner of a backup (Note: Only DRMFree Content will run on incorrect accounts!)

3. Extract and Create Backup Files

4. EasyInstallers, Enables you to easily install, Hidden Applications, ARK-2, VHBL Whitelist Hack, URICaller

5. Account Mannager, save multiple accounts's AID, and KEY's

6. Reading Param.SFO File To display backup NAME instead of TITLEID

7. CMBACKUP Files (These are kinda like what .pkgs was with package installer 2.0 only done right and not in a way that will confuse everyone!)

I also have a few features planned such as:

1. Some sort of progress bar/indicator (This will be hard to do. as extracting / repacking is handled by PSVIMGTOOLS CLI)

3. A Server Where You Can Upload/Download DRMFree Backup Files.

4. Supporting Other CMA's (DevkitCMA, OpenCMA, and OfficalCMA)

Features i want, but arent possible yet:

1. Creating Backup Files From .pkg Files

2. Option To Decrypt PFS.

Upcomming:
1. EasyInstaller for PSM Runtime Skype, and Remove The Featured App.
2. Updated ARK-2 Easyinstaller.

Common Problems:
1. It doesnt open

This could be for a whole lot of reasons.
but the two most common reasons ive seen is the following:
you dont have QCMA installed.
if you do have QCMA installed, the SECOUND most common reason:
is that you have never connected your PSVita with QCMA before
just plug in the USB Cable and wait for it to detect it, (you can also connect via WIFI)

it should also be noted that it might cause a problem if it is your first time running the program however you do not have internet access (or access to cma.henkaku.xyz) this might cause a problem like this as well.

If your problem is something other than these, please open an issue on this github.

For noobs: No this doesnt enable piracy, (except for epsp..) And No this isnt going to lead to a 3.63 spoof for games or PSN.
you cannot run vita homebrew with this (only psp) hidden applications and uricaller dont acturally execute any applications.

2. The titles of games are not displayed correctly

Known bug allready only seems to effect some computers and i cant seem to replicate the bug.
it doesnt acturally effect functionality though. it will still work..
