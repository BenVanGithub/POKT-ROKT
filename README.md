# POKT-ROKT

![Rocket](/ROKT2.png)
Format: ![Alt Text](url)

![Rocket](/ROKT1.png)
Format: ![Alt Text](url)

Release notes: POKT-ROKT  Version 1.0

This is the last release of the ROKT in Bash.  All future development will be done in GO.

Cool stuff this release:
1.) A mini-wallet which allows for transfer of funds from the local validator to any address in the external list.  Command = "SEN"
2.) SSH connect from inside the ROKT to any device on the external list. Command = "T##"
3.) Round-trip latency report between local validator and 0001 & 0021 data sources. Command = "DIR"
4.) Show expiry date of security certificate of local node.  Command = "CER"

Other semi-cool.

1.) supress warnings for timed out querys.  Keeps the screen clean.

Enjoy.
Backup your old copy or the validator list before putting this script on top of it.

NOTE: format of external validators has changed slightly, "username" filed added.  Just put "none" or whatever if you don't plan on using the SSH connect feature.

Version 9.C  2020/09/28
- fixed intermittant issue causing external nodes to appear 
  unjailed when they were jailed.
- several display field size adjustments
- other minor display fixes

Install instructions:  It is a single bash script with no dependencies.
copy paste the commands below:


cd ~  
git clone https://github.com/BenVanGithub/pokt-rokt.git  
cd pokt-rokt  
chmod 755 ./*.sh  
cd ~  
cp ~/pokt-rokt/rokt.sh ~  
./rokt.sh  
