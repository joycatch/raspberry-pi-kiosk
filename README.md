# raspberry-pi-kiosk

Information about the autostart configuration file can be found on:
- https://wiki.lxde.org/en/LXSession#Autostarted_applications_using_lxsession

In short, this file stores the commands that will be executed at the beginning of the session. It is not a shell script, but each line represents a different command to be executed. If a line begins with @, the command following the @ will be automatically re-executed if it crashes. Lines beginning with # are comments.

Commands globally executed are stored in the /etc/xdg/lxsession/&lt;profile&gt;/autostart file, and in addition, other commands can be locally specified in the ~/.config/lxsession/&lt;profile&gt;/autostart file. If both files are present, only the entries in the local file will be executed.
