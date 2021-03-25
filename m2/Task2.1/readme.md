<h2>PART 1. HYPERVISORS </h2>
<p> 1.	What are the most popular hypervisors for infrastructure virtualization?</p>
<p>Azure Virtual Machines, VMware vSphere Hypervisor, Oracle VirtualBox, Microsoft Hyper-V,  ESXI, Citrix XenServer, 
SQL Server on Virtual Machines, Citrix Hypervisor</p>

<p>2.	Briefly describe the main differences of the most popular hypervisors. </p>
<p>Main different are  operating systems  (also spead and memory), where located . device drivers -inside the host operating system or outside, functionality, security issue, differet kind of storage, database, architecture, network cooperation, support and others</p>

<h2>PART 2. WORK WITH VIRTUALBOX</h2>
<p>  I set-up  VirtualBox, created Virtual machine and set upthe latest stable version of Ubuntu Desktop or Ubuntu Server from the official site  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/VM.jpg)

<p>2.(1.3- 1.5) Research diferent feacher  of VW and find out how to use them:

 
start, stop, reboot, save state, use Host key and keyboard shortcuts, mouse capture, etc.  Make clon VM </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/Дод.jpg)

<p>3. (1.7, 1.8)   Snapshots  can save your machine and you always can used them  in order to insure you next action. You can recover your machine at some point.The next stap: exported VM1 *.ova -its look like beckup  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/Зрізи.jpg)
  
<p> 4.(2) Worked with Virtual machine, investigated a lot of figur and setting, network with Host, between VM and in different occasions </p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/USB.jpg)

<p> network </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/network.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/nettools.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/ping.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/спільнітеки.jpg)

<p> 5. Also we can manage our machine from CLI through VBoxManage and examand all simple possible commands.  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/Cli.jpg)


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/cmd3.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/cmd55.jpg)


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/cmd55.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrins/cli2.jpg)


<h2>PART 3. WORK WITH VAGRANT     </h2>

<p> 1. Vagrant is a tool that create environments and allow us to create differant type of system with different operation system and settings. We can manage them and it can  help maximize the productivity and flexibility of our proceeder and activities  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/vagrantsetup.jpg)

<p>2. 3. Powershell give us possibilities automatisation task and managing from their environment.
 I fined and created box:</p>
 
 ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/установкабокса.jpg)
 
 4. Run Vagrant up:

 ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/3.jpg)
 
 ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/vagrantup.jpg)
 
 5.Connect to the VM using the program PuTTY which allows us take remote control on our VM
 
 ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/вхідзпутті.jpg)
 
 
<p>6.the date command was:</p>
  
  ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Vagrant/data.jpg)
  
<p>7. Next sstep was  Stop and delete the created VM with commands:</p>
<p>PS E:\Khrystyna> vagranthalt</p></p>
<p>PS E:\Khrystyna> vagrant destroy</p>


<h2> 8. Create your own Vagrant box   </h2>
<p> 8.1 The first step was create VM with ico file Centos 64 (http://mirrors.nav.ro/centos-altarch/7.9.2009/isos/i386/)</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/1установка.jpg)

<p> Instalation: </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/2установкацент.jpg)

<p> 8.2 Check main tolls and install additional option</p>
<p> Service sshd status: </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/установкасент3.jpg)

  ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/установка4.jpg)

<p> Improve our running : </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/настроки5.jpg)

<p> 8.3 get Disable some function</p>

<p>stop firewalled</p>
<p>SeLinux disable</p>

<p>Update system – yum update</p>
<p>Set up  extra  features: yum install net-tools and systemctl reboot</p>

  ![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/додатковіПакети.jpg)


<p>Set up Network <p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/порт.jpg)

<p>And create my own Box</p>
<p>8.4 create direction and added vagrant package:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/NewBox.jpg)

<p>Create new box: vagrant package –base Centros</p>
<p>Aded Box:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/boaadd2.jpg)

<p>Then init:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/boaadd2.jpg)


<p>The last one: vagrant up</p>

<p>  Checke current list: vagrant box list</p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.1/Scrin2.8/box3Yes.jpg)

<p>Launch the machine !</p>
<p> Thank you for attention !</p>




