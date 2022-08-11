`sudo vnclicensewiz`

running 
`sudo vncpasswd -service` 
then typing the password you will use for connection to the vnc server

editing 
`/root/.vnc/config.d/vncserver-x11`
file as root

adding 
`Authentication=VncAuth`
to the end of the file

restarting vncserver service - 
`sudo systemctl restart vncserver-x11-serviced.service`
