# zabbix_web_certs
The template to monitor TLS/SSL certificate on the website by Zabbix agent 2 that works without any external scripts.
Install zabbix-agent2 and stop zabbix-agent
```
apt install zabbix-agent2
```
```
systemctl stop zabbix-agent
```
```
systemctl start zabbix-agent2
```
Create Host for website

Host name
```
hungry-howard.com
```
Select the template
```
Website certificate by Zabbix agent 2
```
Interfaces  
```
{$CERT.WEBSITE.HOSTNAME} - value=hungry-howard.com
```
```
{$CERT.WEBSITE.IP}- value=192.168.1.112
```
```
{$CERT.WEBSITE.PORT}- value=443
```
Click update button.
 
Go to Monitoring --> Hosts

Click latest data from that host

