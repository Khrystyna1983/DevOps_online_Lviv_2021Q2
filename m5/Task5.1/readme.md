<h2>Task1.Part1</h2>
<p>1.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/1root.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/masterm5/Task5.1/scrin1/1root2.jpg)

<p>2. Less /etc/passwd</p>
<p>/etc/passwd  - information about users</p>
<p>/etc/shadow  - about password</p>
<p>Changed password:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/2paswd.jpg)

<p>3.We can use information for users in files less /etc/passwd and see available users, the same we can notice information for group </p>
<p>less /etc/group, We can get this list without wading through the entire "/etc/passwd" by typing:
</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/3.2.jpg)

<p>The "w" command is a simple way to list all of the currently logged in users, their log in time, and what the command they are currently using
</p>
<p>The “who” we can see all active users. In order to know the access to files you can use command:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/3.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/3.4.jpg)

<p>We can change access by using command:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/3.5.jpg)

<p>Or cut access:</p>
<p>chmod go-rwx test5</p>
<p>Also you can use sudo chage -l users, that give you more information about log and account</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/3.6.jpg)

<p>4.Personal information we can find in file /etc/passwd in filed GEGOS. First of all insaled finger)</p>
<p> Personal information can be changed  by using command : chfn and usermod</p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/4.1.jpg)

<p>Checked  the list:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/4.3.jpg)

<p>We  can change users full name: sudo chfn -f "Khrysyna" kh . Reboot and:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/4.4.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/4.5.jpg)

<p>We can change : sudo usermod -c "Khrystyna”,24,2407197,2522016,Linux Administrator" kh</p>

<p>5.We can use different command help</p>
<p>-	help -m cd-  view all available information of the cd command as the man command display ; help -d cd; -	help -s cd -show command, option and argument- how to use this command, shows the output;help help ; which cd, which passwd  </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/5.2help.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/5.4.jpg)

<p>We can use the following command to view all available internal commands.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/5.3internalcommand.jpg)

<p>man -k cd – return the command in wich find this “cd”</p>
<p>man -f [COMMAND NAME] – give us an option for command </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/5.6.jpg)

<p>6.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/6.1less.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/6.2.jpg)

<p>We can view the contents of files .bash* using  less .bash* </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/7.3bash.jpg)

<p>7. echo "I am working on laboratory work 1." > ~/.plan</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/7.1.jpg)

<p>8.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/8.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/8.2.jpg)

<p>Home consist</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/8.3home.jpg)

<p>In order to find all the catalogs we use:</p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin1/8.4.jpg/m4/Task4.2/1.gif)

<h2>Task1.Part2</h2>

<p>1. sudo apt-get install tree</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/1.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/1.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/1.3.jpg)

<p>List subdirectories of the root directory up to and including the second nesting level- I used command list -R</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/1.4.jpg)

<p>2. We can find out by using file:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/2.1.jpg)

<p>relative path</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/3.2относительний.jpg)

<p>absolute paths</p>


![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/3.1повний.jpg)

<p>Come back to home</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/3.3.jpg)

<p>Or cd /</p>
<p>4. ls command : ls /etc – list file, ls -l – file permission, size.date and time; ls -la -show hidden files, ls.., ls -d */ command to list only directories; ls -R command to list all files and directories with their corresponding subdirectories down; ls -s – list file with their size</p>
<p>Ls-l - permition, number of links, owner, group owner, 10-size in bytes, last modified date, file or directory name</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/4.1ls-l.jpg)

<p>ls -a command to list files or directories including hidden files or directories;
ls -l -a – the same calums and “.” With hiden files
</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/4.2ls-l-a.jpg)

<p>5.Created subdirectiry</p>
<p>Mkdir ~/New</p>
<p>Touch Myfile.txt</p>
<p>Done output and view the information</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/5.1.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/5.3.jpg)

<p>Copy file:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/5.4copy.jpg)

<p>Delete the files and subdirectiry</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/5.5rm.jpg)

<p>6.mkdir ~test</p>
<p>Copy:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/6.1copy.jpg)

<p>Created hard and soft link</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/6.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/6.3.jpg)

<p>We can defind hardlink using “ls -l”. but it renamed the origin file 
If we talk about soft link, we can see all the information and can notice that.
</p>
<p>Renamed link:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/6.4.jpg)

<p>Deleted the labwork2 – soft link  become broken, but hard link have still existed, because  hard link – is a copy (backup) our file, we should deleted link too.</p>
<p>7.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/7.1.jpg)

<p>8.lsblk show us this information</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/8.1.jpg)

<p>9. I used wc -l:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/9.1.jpg)

<p>10. find /etc/ -iname "host" </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/10.1.jpg)

<p>11.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/11.1.jpg)

<p>12.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/12.1.jpg)

<p>13.There are type of devises:</p>
<p>•	c - character</p>
<p>•	b - block</p>
<p>•	p - pipe</p>
<p>•	s – socket</p>
<p>We can see this information by using:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/13.1.jpg)

<p>14.I used df -TH</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/14.1.jpg)


<p>15.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.1/scrin2/15.1.jpg)

<p>Thank you for your attention :)</p>



