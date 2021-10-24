# raspberry-pi-kiosk

Do you want to setup a raspberry-pi to automatically enter kiosk mode after it has booted up? Well, then you have come to the right place because this repository holds example files that can be used to accomplish just that. All you need to do is to update the so called autostart configuration file on your raspberry-pi as this is the file that manages the applications which are started on login.

## Instructions

Simply replace the URL (https://www.raspberrypi.org/) in the autostart file with the URL that you want.

## Additional information

 Information about the autostart configuration file can be found on:
 - https://wiki.lxde.org/en/LXSession#Autostarted_applications_using_lxsession

> In short, this file stores the commands that will be executed at the beginning of the session. It is not a shell script, but each line represents a different command to be executed. If a line begins with @, the command following the @ will be automatically re-executed if it crashes. Lines beginning with # are comments.
>
> Commands globally executed are stored in the /etc/xdg/lxsession/&lt;profile&gt;/autostart file, and in addition, other commands can be locally specified in the ~/.config/lxsession/&lt;profile&gt;/autostart file. If both files are present, only the entries in the local file will be executed.
