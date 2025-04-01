<h1>Evaluating the Efficacy of Suricata and Zeek in Ethical Hacking</h1>

<h2>Description</h2>
This project tested and compared the performance of Suricata and Zeek in detecting realtime cyber threats. Security Onion was used to monitor simulated attack traffic, including SQL injections and XSS attacks. 
<br />

<h2>Technologies used</h2>

- <b>IDS tools: Security Onion</b> 
- <b>Attacks Techniques: SQL Injection, XSS</b>

<h2>Environments Used </h2>

- <b>Metasploitable 2/DVWA</b> (Target Machine)
- <b>Security Onion</b> (Network Monitor)
- <b>Kali Linux</b> (Attacking Machine)
<h2>Project Documentation:</h2>

<p align="center">
Simulated environment on VMWare: <br/>
<img src="https://i.imgur.com/kKTgcUR.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Figure 2: Burp Suite intercepting the request of the webpage. <br/>
<img src="https://i.imgur.com/uIuXdRJ.png" height="80%" width="80%" alt="Project Steps"/>
<br /> 
<br />
Figure 3: Sql map identifying the injection points and type of SQL injection attack possible. <br/>
<img src="https://i.imgur.com/f9CcGSJ.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Figure 4: Results of sqlmap on the previous parameters. <br/>
<img src="https://i.imgur.com/SdAfHqU.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Figure 5: sqlmap --dump command. <br/>
<img src="https://i.imgur.com/3ENaT2f.png" height="80%" width="80%" alt="Project Steps"/>
<br />
<br />
Figure 6: Retrieved data from the DBMS. <br/>
<img src="https://i.imgur.com/CaBCwN2.png" height="80%" width="80%" alt="Project Steps"/>
<br />
The passwords have been cracked for admin, gordonb, 1337, pablo,  and the table “users” have successfully been dumped into the terminal with the information gathered. 
<br />
<br />
<br />
Figure 7: Users showing online <br/>
<img src="https://i.imgur.com/HSgeJEf.png" height="100%" width="100%" alt="Project Steps"/>
<br />
This image shows the users being online after inserting the <script> beef-shortened-url:3000<script>. The target machine successfully became one of the machines using the hooked browser which we then could input various attacks.
<br />
<br />
<br />
Figure 8: List of the potential commands we could execute <br/>
<img src="https://i.imgur.com/2Klyvs3.png" height="100%" width="100%" alt="Project Steps"/>
<br />
<br />
<br />
We executed one of the commands which was the Man in the Browser command. This allowed us to intercept all the user's web traffic gaining any inputs they entered. The attack would stay until the user changed the URL address on the browser. From the results you see we were able to get the traffic and even a username and password that was entered from the other machine.
<br />
<br />
Figure 9:  <br/>
<img src="https://i.imgur.com/K46LagZ.png" height="100%" width="100%" alt="Project Results"/>
<br />
<br />
Figure 10:  <br/>
<img src="https://i.imgur.com/7Q334bd.png" height="100%" width="100%" alt="Project Results"/>
<br />
<br />
Figure 11:  <br/>
<img src="https://i.imgur.com/ekpZ3Lj.png" height="100%" width="100%" alt="Project Results"/>
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
