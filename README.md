# check_sap_shortdumps.py
Nagios plugin for checking SAP Short Dumps in last two days

![](/images/check_sap_shortdumps2.png)

![](/images/check_sap_shortdumps.png)


Usage:./check_sap_shortdumps.py \<SID\> \<warning shortdumps\> \<critical shortdumps\>

Example:

root@:~/github# ./check_sap_shortdumps.py SBX 10 20

OK: ShortDumps in last two days -w 10 -c 20: 0 | ShortDump=0


                                                                      
### Prerequisite:
https://github.com/piersharding/python-sapnwrfc

### Wiki:
Installation of sapnwrfc for python on Linux and Unix
https://wiki.scn.sap.com/wiki/display/EmTech/Installation+of+sapnwrfc+for+python+on+Linux+and+Unix






To prepare a script, you'll need a 'yml' file similar to the 'sap.yml' file included with the sapnwrfc download. The file looks 

like this:
#### Example of SID.yml file

ashost: gecko.local.net

sysnr: "01"

client: "001"

user: developer

passwd: developer

lang: EN

trace: 3

loglevel: warn
