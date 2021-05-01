<p>1.Created 3 VM - VM1-NAT and local network, VM2 and VM3 only local network</p>
<p>2.By adding VboxManage  we  can create DHCP server :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/1.1PSH.jpg)

<p>Then type name in local host :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/1.2.jpg)

<p>Setting machine  auto enp0s8
</p>
<p>iface enpos8 inet dhcp</p>

<p>Or request ip address by typing: "sudo dhclient enp0s8"</p>
<p>And get address:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/1.3last.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/1.4ping.jpg)


<h4>DNSmasq dhcp server</h4>
<p>typed "sudo apt update"</p>
<p>And instaled server</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.1.jpg)

<p>Corrected file and type interface from which we share Ip-address</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.2vm1in.jpg)

<p>Configurede some information in  /etc/dnsmasq.conf</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.3conf.jpg)

<p>sudo systemctl restart dnsmasq</p>
<p>Status Dnsmasq :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.6.jpg)

<p>Start VM2 and VM3 and set up interfaces like this:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.7vm23.jpg)

<p>3.Checked VM2 and VM3 for obtaining network addresses from DHCP server. </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/3.1.jpg)


<p>4.DNSmask  server have been installed in point 2 </p>
<p>Investigated information about serves:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.4.jpg)

<p>And typed this in  /etc/dhcp/dhclient.conf:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/2.5.jpg)


<p>5. Give permition for out network</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/4.1.jpg)

<p>Check connection </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/4.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/4.3.jpg)

<p>Changed Hostname</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.1hostname.jpg)

<p>Corrected some information at /etc/dnsmasq.conf</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.2conf.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.3conf.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.4.jpg)

<p>Then typed addresses in /etc/hosts:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.5hosts.jpg)

<p>And checked VM2, VM3</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m6/Task6.2/Scrin/5.6dig.jpg)

<p>Thank you for your attention ! Have a greate day!</p>
<p></p>

