# serverinstall
Install Remotend Server



# How to Install the server

Make sure you have got access via ssh or otherwise setup prior setting up the firewall, command for UFW is:
```
ufw allow proto tcp from YOURIP to any port 22
```

If you have UFW installed use the following commands (you only need port 8000 if you are using the preconfigured install files):
```
ufw allow 21115:21119/tcp
ufw allow 8000/tcp
ufw allow 21116/udp
sudo ufw enable
```

Run the following commands:
```
wget https://raw.githubusercontent.com/remotend/serverinstall/master/install.sh
chmod +x install.sh
./install.sh
```

Follow the options given in the script.
