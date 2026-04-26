# CHEFT
A bash script to make easy work of dealing with encrypted folders on Crostini Linux environments

It is presented with absolutely no warranties or assurances. Use this script at your own risk.

It is presented here as a simple .txt file, keep reading for a mini tutorial to install/setup the script. In my example the cheft.rev1.txt

***Tutorial***
1) Download cheftrev1.txt to Downloads, and copy it over to your "Linux files" in the chromeOS files app.
2) Open the linux development environment and find your file. On my system it is /home/g2k/cheftrev1.txt
3) Now copy the file and rename it to whatever you choose or keep the original name. The command to do this is:
sudo cp /home/g2k/cheftrev1.txt  /usr/bin/cheft
4) Next comes the initialization process. To make the script useable you must initialize it with:
sudo chmod +x /usr/bin/cheft
5) Simply type cheft into the terminal and it should perform the first run dependency check and the "Backup your "key file" 1st time nag message. after that it'll just open the program.
6) EOF

