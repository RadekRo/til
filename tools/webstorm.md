# WebStorm

__Updating problem__

Issue:
`Update. WebStorm does not have the permission to 
write to /opt/WebStorm(...).`

Solution:
`sudo chown -R $USER:$USER /opt/Webstorm(...)`

This command will change the user permissions
to read/write to WebStorm dir to your current
active user. 
---
_Last update: 15 Mar 2018_ 