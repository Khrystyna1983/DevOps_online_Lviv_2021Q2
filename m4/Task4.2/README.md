<p>1.Simulated a corporate network  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/Scrin/1.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.gif)

<p>Tested by pushing complex PDU:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1Complexpdu.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.4ComplexPDU.jpg)

<p>and other reports and testing trafic:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/1.3.jpg)

<p>2.I've done a few schemas) prectise)</p>

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

<p>Also I could implemene two different subnets by using L3 multyswitch -  it has completed in task 4.3 - you are able to see this)</p>

<p>3. I tried  to completed this task by using different ways too)</p>

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

<p>Set up PC</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/3.jpg)

<p>Came back to Multilayer switch and creayed one more vlan for our router, gave ip address for new vlan and access:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/4swtorout.jpg)


<p>SET up our router, gave it ip in the vlans(7) network</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/5router.jpg)

<p>and create routing</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/scrinnew/6routing.jpg)

<p>My schemas:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/2.3майже.gif)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m4/Task4.2/4.2last.gif)

<p>But still dont work connection with router - maybe, I should set up interfaces in router too or find out another way - I will come back to this task </p>


