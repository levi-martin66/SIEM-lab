# SIEM-lab

<h2>Description</h2>
In this lab, I set up Azure Sentinel (SIEM) and connected it to a live virtual machine acting as a honeypot. We will observe live attacks (RDP Brute Force) from all over the world. We will use a custom PowerShell script to look up the attacker's Geolocation information and plot it on the Azure Sentinel Map! 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b>
- <b>Microsoft Sentinal</b>
- <b>Microsoft Azure</b> 


<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
creating and launching the virtual machine: <br/>
<img src="https://imgur.com/JcyHSsr.png" height="80%" width="80%" alt=>
<br />
<br />
create log analytic workspace:  <br/>
<img src="https://imgur.com/oHa88rU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
connect Microsoft Defender: <br/>
<img src="https://imgur.com/5e7kB2h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
now on the VM confirm event logs:  <br/>
<img src="https://imgur.com/0iDs5I0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
disable the firewall of the VM:  <br/>
<img src="https://imgur.com/Xa7sHSJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
ping the VM to confirm it is findable on the internet:  <br/>
<img src="https://imgur.com/HjP0ACS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
create the program in power shell that communicates the log data in the VM with our SEIM tool:  <br/>
<img src="https://imgur.com/Vr8G94P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
create a custom log to enter all the information from the SEIM:  <br/>
<img src="https://imgur.com/8YNoDBB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
go through the sample logs and calibrate the SEIM tools detection system:  <br/>
<img src="https://imgur.com/fsJrOEl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Here is a list of all the custom logs I created:  <br/>
<img src="https://imgur.com/oDjhvGe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
this is what the dashboard looked like at the start of the test:  <br/>
<img src="https://imgur.com/UiEg0jj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
here are some examples of some of the brute force attacks I logged:  <br/>
<img src="https://imgur.com/wV89jiO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
after just 18 hours, there were around 10,000 login attempts from all over the world:  <br/>
<img src="https://imgur.com/pZHcTlm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<h2> conclusion </h2>
In this lab, we can see the importance of proper security measures like firewalls, strong passwords, and usernames and even how two-factor authentication could have been useful. It also shows us how real the threat is when we have a computer that is open to the world on the internet.


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
