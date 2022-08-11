## Install Real

## Run these to fix the permissions:
`sudo vnclicensewiz`

`sudo vncpasswd -service` 

`sudo nano /root/.vnc/config.d/vncserver-x11`

and add this to the end of the file:

`Authentication=VncAuth`

Then restart the service, and your done:

`sudo systemctl restart vncserver-x11-serviced.service`

## Refrence:
https://help.realvnc.com/hc/en-us/community/posts/5313103951517-No-Authentication-Schemes-Configured

https://help.realvnc.com/hc/en-us/articles/360002253878-Configuring-VNC-Connect-Using-Parameters#populating-vnc-configuration-files-with-parameters-0-2 

https://help.realvnc.com/hc/en-us/articles/360002251297-VNC-Server-Parameter-Reference-#Authentication

the program for option settings (vncserverui) cannot be run directly from terminal but you can adjust every possible option manually with the help of the above links
