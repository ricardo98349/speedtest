### Descomentar a linha no arquivo do zabbix

nano /etc/zabbix/zabbix_server.conf

#ExternalScripts=/usr/lib/zabbix/externalscripts

para

ExternalScripts=/usr/lib/zabbix/externalscripts

---

### descomentar a linha no arquivo zabbix_agentd

nano /etc/zabbix/zabbix_agentd.conf

#	1 - AllowKey=system.run[*]

para

AllowKey=system.run[*]

---


apt-get update


### instalação do speedtest-cli

wget https://raw.githubusercontent.com/ricardo98349/speedtest/main/speedtest.py -O speedtest-cli

chmod +x speedtest-cli

mv speedtest-cli /usr/bin/speedtest-cli

speedtest-cli

---------




chown zabbix.zabbix /usr/lib/zabbix/externalscripts/speedtest.sh
