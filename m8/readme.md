<h1>JENKINS</h1>
<p>I tried to gather artifact from GIThub and deployed to Apach server, I also I tried Pipeline. And I want to try all the approaches, if I will have enought  time)</p>

<p>Install Jenkins on VM1:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/0.1setup.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/0.2setup.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/0.3.jpg)

<p>VM2(Server) - instaled apach2 </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/0.7apach.jpg)

<p>Checked status Apach, enable, allowed port 8080</p>
<p>Created ssh- keygen and copied public key to another VM2 (Server Apach)</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/0.6ssh.jpg)

<p>Gave access for your user(who will push) on Server to dir var/www/html </p>

<p>Created repository at GIThub  - by Git pushed my file  into repo </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.1develop.jpg)

<p>Copied public  key fom VM with jenkins (id_rsa.pub) to Github </p>
<p>Checked my connection from VM</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.3connection.jpg)

<p>We also can connet to GitHub from our Virtualmachine  by ssh-connection - Cloned git project, if our Developer has worked on Ubuntu )) - second way of integretion:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.4.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.5.jpg)

<p>And do push and pull, but I have already done this from windows)</p>

<p>Configured jankins:</p>


<p>Let’s checked our job:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/4.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/4.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/4.3.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/4.4.jpg)

and General configuration:

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/5.1mainconfiguration.jpg)

<p>My job has worked:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.6build.jpg)

<p>And result (VM2-server):</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/5.2.jpg)

<p>I have worked also with simple Pipeline job - connection with github, created jenkinsfile and pull, puch :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/2.1pipeline.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/2.3.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/2.4.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m8/Scrin/1.7result.jpg)


<p>Thank's</p>


