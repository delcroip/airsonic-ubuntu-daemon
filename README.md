# airsonic-ubuntu-daemon
Files to create an airsonic daemon with the standalone WAR in Ubuntu
the default port is 4041 in order to leave 8080 for Tomcat


1- install the files in your system

<code>/etc/default/airsonic</code> file to set the default for the /etc/init.d/airsonic script

<code>/etc/init.d/airsonic</code> script the manage the start, stop, restart, status commands

<code>/usr/bin/airsonic</code> script to launch Java with the right parameters

2- run those commands:

 <code>
 sudo update-rc.d airsonic defaults
 sudo service airsonic start
</code>

Todo:
Make sure all the params in the etc files could are actually sent to the usr one.
