# wazuh-gotify
Gotify integration for Wazuh. notifiations

## Creating custom integrations
-    create copy script to a file named ```custom-gotify``` at ```/var/ossec/integrations/```   
  (Example: as root ```nano /var/ossec/integrations/custom-gotify```)
-    Modify access flags: ```chmod 750 /var/ossec/integrations/custom-gotify```
-    Change owner of script: ```chown root:wazuh /var/ossec/integrations/custom-gotify```

## Adding integration to manager ossec.conf
Example configs:
```
  <integration>
    <name>custom-gotify</name>
    <hook_url>https://gotify.example.com</hook_url>
    <api_key>VERYSECRETKEY</api_key>
    <alert_format>json</alert_format>
    <level>8</level>
  </integration>
  
  <integration>
    <name>custom-gotify</name>
    <hook_url>https://gotify.example.com</hook_url>
    <api_key>VERYSECRETKEY</api_key>
    <alert_format>json</alert_format>
    <rule_id>504, 506, 503</rule_id>
  </integration>
```
