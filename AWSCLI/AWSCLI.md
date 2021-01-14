##Upgrading from AWSCLI to AWSCLI2

If you're upgrading your machines from AWSCLI to AWSCLIV2 please add the following to your override.
For a regular install there is no need to add this.

```xml
<key>preinstall_script</key>
<string>#!/bin/sh

sudo rm -rf /usr/local/aws
sudo rm /usr/local/bin/aws

exit 0
</string>
```