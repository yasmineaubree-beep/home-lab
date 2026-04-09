<h1>home-lab</h1>
<bold>07 april 2026</bold><br>
1st repository
<h2>Objectives:</h2><br>
- trying to get familiar with github.<br> 
- archiving and keeping track of my projects (steps by steps, before/after, issues and ways I found to fix them, etc)<br>
- building a portfolio<br>
<h2>Details:</h2>
<p>
<h3>Hardware :</h3> M710q Lenovo (tiny)
<h3>OS:</h3> Debian12, netinst 
<h3>Hostname:</h3> NAS
<h3>Learning goals:</h3> NAS server, getting to know python and docker</p><br>

Log 08/04/26: Remote access configuration_SSH<br>
Current status:<br>
Attempting to establish an ssh connection from my laptop (lenovo T430) to the NAS server (M710q)<br>
Server IP: 192.1XX.X.XX<br>
User: [redacted] user and root<br>

Issue encountered:<br>
While physical access (keyboard/monitor connected to tinypc) works perfectly with the credentials noted in my notebook, remote connection via SSH is being rejected. <br>
Error messages: 'Connection closed by 192.XXX.X.XX port 22' and 'permission denied, please try again.'

Solution: Reconfiguring the SSH daemon policy on the host (Debian12), I enabled secure password-authenticated access from my local machine (by removing the hash before the targeted line). The server is now fully operational in headless mode, allowing for decentralized admin and development.

Result : 1st Successful implementation of remote management via SSH.
yipee!!:P
(I turned the activity monitor on by putting 'top' in the terminal of my laptop as the first remote command)
