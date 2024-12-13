<h1>Updating Palo Alto Firewall</h1>


<h2>TLDR Description</h2>
Updating a Palo Alto 220 firewall to the most recent version
<br />

<h2>Purpose</h2>
The purpose of this lab is to update the Palo Alto 220 Firewalls to be on the latest software version, 10.1.4, so we are able to proceed with configurations at the most recent and relevant version. 
<br />


<h2>Lab Summary</h2>
To update the palo altos we had to be on the most recent dynamic update/firmware and then I was able to move up from 9.1.4 to 9.1.12 and from there to 10.0.0 
 -> 10.1.4. This wasn’t that difficult of a lab as the GUI made the process rather simple but I did run into an issue of licensing while trying to update from 9.1.12 to 10.0.0, but after I went to the licensing tab in the GUI and retrieved the license information it quickly resolved that issue and I was able to move forward without problems. This lab consisted of a lot of waiting as it takes roughly 15-20 minutes for the firewall to reboot with the latest version after installing, and that was on top of the fact that with Palo Alto’s I’m unable to directly update to the latest version but instead have to update in increments like stated above.
<br />


<h2>Network Diagram</h2>
<p align="center">
  <img src="https://i.imgur.com/JG4RBcT.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Walk-Through:</h2>

<p align="center">
Find the update you need, and click download<br/>
<img src="https://i.imgur.com/2iquiCf.png" height="80%" width="80%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Patiently wait for download to finish<br/>
<img src="https://i.imgur.com/9BKEmbl.png" height="80%" width="80%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Once download is complete we need to install<br/>
<img src="https://i.imgur.com/RW8zRu7.png" height="80%" width="80%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Patiently wait for installation to finish<br/>
<img src="https://i.imgur.com/GKLfrhS.png" height="80%" width="80%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Once installation is done confirm with reboot<br/>
<img src="https://i.imgur.com/Huc4zyk.png" height="65%" width="65%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Patiently wait for reboot to finish and we are all done<br/>
<img src="https://i.imgur.com/02OtyLn.png" height="65%" width="65%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
</p>

<h2>Problems</h2>
The issue I was faced with was an error that read “Failed to fetch licenses” which at first had me stumped as I had never seen an error like that before but as I went to check the Licenses tab in the GUI I quickly realized that I had not retrieved any licenses for the firewall up to that point. All I had to do to fix this problem was simply click “Retrieve license keys from license server” and wait to let it load. After it loaded, I tried to update again and had no issues.
<br />
<p align="center">
Error:<br/>
<img src="https://i.imgur.com/BI1hrTP.png" height="40%" width="40%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
Solution found: Clicking “retrieve license keys from license server”<br/>
<img src="https://i.imgur.com/nlGU1Jx.png" height="80%" width="80%" alt="Palo Alto Firewall Factory Reset Steps"/>
<br />
<br />
</p>

<h2>Conclusion</h2>
In this lab I successfully updated my palo alto 220 firewall to the most recent version 10.1.4 after getting confronted with unforeseen problems with licenses and tackling the virtue of patience, which I required a lot of to complete this lab. It took multiple days to wait through booting with new updates and repeating the process until I was finally at the most recent version.
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
