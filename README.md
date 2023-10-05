<img src="https://i.imgur.com/fzR6nTr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>


<h1>TCPDump Project: Network Traffic Analysis</h1>

I'll be using the TCPDump Visualizer, a tool that helps make sense of network data by capturing, filtering, and presenting it in an easy-to-understand way.


<h2>Anazlyze network traffic on Terminal w/ TCPDump</h2>

- Open terminal to start using TCPDump


<img src="https://i.imgur.com/VbHO2ui.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>
<img src="https://i.imgur.com/euLvKm9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Type TCPDump into terminal and see no access because not a sudo user

<img src="https://i.imgur.com/MfBheZ4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Type Sudo TCPDump and now terminal starts to pick up network traffic
- Type ctrl+c to stop traffic

<img src="https://i.imgur.com/7Eatw2H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- If you type man TCPDump you can see the systems manager manual

<img src="https://i.imgur.com/yK3qGMO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- To see only 10 packets at a time we can use the command Sudo TCPDump -c 10

<img src="https://i.imgur.com/BmWy2nd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Sudo tcpdump -c 10 -# to add lines numbers

<img src="https://i.imgur.com/la2ryoz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Shows all network interfaces I have on my workstation.

<img src="https://i.imgur.com/vjhsadO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>



<h2>Shell Script</h2>

- We're going to check the traffic for website skyroute66.com
- We're going to filter it through port 443

<img src="https://i.imgur.com/PUbjgcC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>


- Now I'm going to open visual studio code and select file and open folder
- Select desktop then ok
- Now right click and create new file
- then name it watchdog.sh

<img src="https://i.imgur.com/ftos6Oj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

<img src="https://i.imgur.com/71GEbHT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

<img src="https://i.imgur.com/LZkaWOX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

<img src="https://i.imgur.com/ifI04Mn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Then we're going to type sudo tcpdump -XX for line numbers tttt for readble time then host skyroute.com
- Type sudo tcpdump -#XXtttt host skyroute.com -c 10

<img src="https://i.imgur.com/krOWLCT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>


- Then right click watchdog.sh and open integrated terminal

<img src="https://i.imgur.com/clDmxbi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

<img src="https://i.imgur.com/mCkOtFh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Then ls -al to see the script

<img src="https://i.imgur.com/K2inrzT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>

- Its not exacutable so to make it exacutable type chmod +x watchdog.sh
- Then type ls -al to check

<img src="https://i.imgur.com/K2inrzT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>
<img src="https://i.imgur.com/Cqae6Nv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/></p>










