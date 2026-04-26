# CHEFT
A bash script to make easy work of dealing with encrypted folders. It is intended to run on Chromebooks; utilizing the native Linux Development Environment.

It is presented with absolutely no warranties or assurances. Use this script at your own risk.

It is presented here as a simple .txt file, keep reading for a mini tutorial to install/setup the script. In my example the cheft.rev1.txt file is in my chromebook Downloads folder.

***Tutorial***
1) Download cheftrev1.txt to Downloads, and copy it over to your "Linux files" in the chromeOS files app.

2) Copy the .txt file to "Linux files" folder. The "Linux files" folder is /home/YouruserName/, sometimes it is found at: /home/YourUserName/Downloads

3) Open the linux development environment and find your file. On my system it is /home/g2k/cheftrev1.txt

4) Copy the file to /usr/bin and rename it to cheft. The command to do this is:
sudo cp /home/YourUserName/cheftrev1.txt  /usr/bin/cheft (or whatever name you call it)

5) Next comes the initialization process. To make the script useable you must initialize it with:
sudo chmod +x /usr/bin/cheft after this, if you simply type cheft into the terminal, and hit the enter key,it'll launch.

It should perform the 1st run "dependency check" and the "Backup your key file" reminder message. The first run reminder message only runs the first time the app launches.

NOTE: Once a vault is open you can interact with the files and folders on it using:
1) Chromebook files app.

The encrypted vaults show up under "Linux files" "Vaults" "STORAGE_DEVICE_NAME"; in the left side pane.
It is a direct connection to the hidden .vault encrypted folder on the external storage device.

The NON encrypted folder is accessed under the "storage device name" in the left panel of the files app.
The Storage device name is the name you see when you plug in a thumb drive, etc.

2) The file manager you have installed on your Crostini Linux terminal. 

The mount points are a little different though.
The encrypted .vault folder is still available at: /home/user/Vaults.

The NON encrypted portion of the thumb drive used to be mapped to: /mnt/chromeos/removable

Now, Google apparently changed it to: /mnt/shared/removable
NOTE: inside /mnt there is still a /chromeos folder that offers: /mnt/chromeos/shared/removable .
The script searches for the first folder it finds called 'removable' inside the /mnt folder.

It then looks inside that folder for external storage devices. It then scans those devices and keeps track of which ones have a .vault folder, and which ones don't.
EOF

