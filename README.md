# Description
ssllabs_checker.sh designed to check certificate grade via open API of Qualys SSLLabs.com. Shell script uses official utility provided by SSLLabs: https://github.com/ssllabs/ssllabs-scan
# Installation
Script should be used together with Zabbix Temaplate available here: https://share.zabbix.com/cat-app/web-servers/ssllabs
* Import Zabbix Template
* Install ssllabs-scan into your zabbix scripts path, pick up latest release
* Install ssllabs_checker.sh script to your zabbix scripts path
* Add Cronjob
# Usage
Please check "Configuration" part of script to configure it according your environment
To run script: `ssllabs_checker.sh example.com`

For Crontab (once per hour):
`0 * * * * /opt/zabbix_scripts/ssllabs_checker.sh www.ssllabs.com`
