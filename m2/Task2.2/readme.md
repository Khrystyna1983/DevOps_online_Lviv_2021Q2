<p>1,2.Made registration in AWS, got AWS Free Tier.Read the terms of Using, instraction and some video on Youtube, read some of documentation and gщt acquainted with services</p>

<p>3. Read the tutorial</p>
<p> Get seting for usrers- created policy, create user, group, set up MFA</p>
<p>4. Created and launched my first instance</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/instance1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/VM1.jpg)


<p>Connect to instance from myPC</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/connectfromPC.jpg)

<p>5.Launched another Linux Virtual Machine</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/SecondInstance.jpg)

Set up Apache

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/apache.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/5vm2.jpg)

<p>6. Made asnapshot of your instance for backup </p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/snapshot.jpg)

<p>7.Created and attached Disk D:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/7extradisk.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/7NewFILEextraDisk.jpg)

<p>check the list Xvdf present</p>
<p>Check what type the disc have file -s /dev/xvdf – no peermision</p>
<p>sudo su</p>
<p>file -s /dev/xvdf</p>
<p>I can added file system : mkfs -t ext4 /dev/ xvdf</p>
<p>Sudo mount /dev/xvdf NewFile – mey new dir</p>


<p>Choose as file system and add file</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/m2/Task2.2/Scrins/7filesystemextraDisk.jpg)


<p>8.Launch the third instance from backup - created AMI from snapshot and launch</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/8AMI.jpg)

or we can create AMI from instanse durectly

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/8Image.jpg)

 and launch fom beckup
 
![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/93-rd_instance.jpg)
 
<p>9. detauch disk D from instance:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/9detauch.jpg)

<p>Lsblk </p>

<p>abd then touch to anoter instance</p>

<p>We can create instance with Wordpress 2 different ways - The first one is  set up apache, turmn off firewall, set up php, mysql server, create mysql client, create a database wordpress,create users and privilages, install and configure wordpress </p>
<p>or we can choos the option of AWS and added word press during our instalation instance - I chose this way and very quicly deleted after that becouce its take charge paid</p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/10addmarketplace.jpg)

<p>11. Create store - action with files and repeted with my new instance</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/11s3_1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/11publicfile.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/11delete.jpg)


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/11.3Altaskwithfile.jpg)

<p>12. Upload files to the cloud to Amazon S3 using the AWS CLI - add user, policy  and connect.  Create user with admin rights, copy new_user_credentials  in order to get accept in console</p>

<p> Download AWC CLI and connect with cmd. Then AWS configure</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/12cli.jpg)

<p>Manage from command line : aws s3 cp backup s3://khrystyna.epamdevops/ </p>
<p>Delete file aws s3 rm s3:// khrystyna.epamdevops /backup.bak</p>

<p>13. I created Elastic IP  in EC2 - Allocate New Address, chose new IP adress and touch to my instance</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/13EIP.jpg)

<p>Didn't work with Route 53 becouse of charges(</p>

<p>15. Create S3 and make Static web-site : <a href="http://khrystyna.epamdevops.s3-website.eu-central-1.amazonaws.com/">https://http://khrystyna.epamdevops.s3-website.eu-central-1.amazonaws.com</a></p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m2/Task2.2/Scrins/15static.jpg)

<p>Welcome <a href="http://khrystyna.epamdevops.s3-website.eu-central-1.amazonaws.com/">https://http://khrystyna.epamdevops.s3-website.eu-central-1.amazonaws.com</a></p>
<p>Thank you for your attention and knowledges that you put in us!</p>




