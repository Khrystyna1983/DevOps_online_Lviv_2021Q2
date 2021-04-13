<h3>1.Simulated a corporate network  </h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/Scrin/1.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.gif)

<p>Tested by pushing complex PDU:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1Complexpdu.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.4ComplexPDU.jpg)

<p>and other reports and testing trafic:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.3.jpg)

<h3>2.I've done a few schemas) prectise)</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/Scrin/2.2schema.jpg)

<p>and</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/2.2anothertype.jpg)

<p>Also I set up DHCP server and share IP  amount PC</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/Scrin/2.1DHSP.jpg)

<p>My work stations:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/2.1.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/2.2.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/2.2anothertype.jpg)

<p>and analised the trafic</p>

<p>Also I could implement two different subnets by using L3 multyswitch -  it has completed in task 4.3 - you are able to see this)</p>

<h3>3. My next work</h3>

<p>Set up my switches and took trunf port and eccapsulation</p>
<p>Created vlans enable
conf t,
valn 2
name VLAN2,
exit
vlan 3
name VLAN3. and so on
</p>
<p>Gave access to the ports and created trunk port</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/1switch1.jpg)

<p>set up L3 switch - gave ip adress for vlans</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/2mainsw.jpg)

<p>Allowed vlans in our ports, use trunk connection</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/2.2main%sw.jpg)

<p>int fa 0/1</p></p></p>
<p>switchport trunk encapsulation dot1q</p></p>
<p>switchport mode trunk</p>
<p>switchport trunk allowed vlan 2,3,4,5,6</p>
<p>exit</p>
<p>int fa 0/2</p>
<p>switchport trunk encapsulation dot1q</p>
<p>switchport mode trunk</p>
<p>switchport trunk allowed vlan 2,3,4,5,6</p>
<p>exit
 <p>...</p>
 <p>ip routing</p>
 <p>do wr mem</p>

<p>Set up PC</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/3.jpg)

<p>Came back to Multilayer switch and creayed one more vlan for our router, gave ip address for new vlan and access:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/4swtorout.jpg)


<p>SET up our router, gave it ip in the vlans(7) network</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/5router.jpg)

<p>and create routing</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/6routing.jpg)

<p>Check ping</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/1last.jpg)

<p>My schemas:</p>
 
![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/4.2last.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/4.2.3.1.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/4.2.3.2.gif)

<p>Or you can watch in youtube:</p>

https://youtu.be/https://www.youtube.com/watch?v=uLdcOSOWmpU

https://youtu.be/https://www.youtube.com/watch?v=YZXkveSHzUs

<p>and check one of massage</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/lastlartcheck.jpg)

<p>Thank you!</p>


