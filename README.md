# wazuh-gotify
Gotify integration for Wazuh. notifiations

## Creating custom integrations
-    create copy script to a file named ```custom-gotify``` at ```/var/ossec/integrations/```   
  (Example: as root ```nano /var/ossec/integrations/custom-gotify```)
-    Modify access flags: ```chmod 750 /var/ossec/integrations/custom-gotify```
-    Change owner of script: ```chown root:wazuh /var/ossec/integrations/custom-gotify```
