<p>1.In file /etc/passwd we see the culums: </p>
<p>user’s name, password (hidden), uid – unique identifier of the user, gid -unique identifier of the group,comment (fullname), directory and shell</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/1.1etcpasswd.jpg)

<p>In file /etc/group we see the culums:</p>
<p>User’s name, password (hidden),groupID (unique number)</p>
<p>Pseudo-users are: daemon (system services proceses), bin (execute some command ), sshd (responsible for remote connection), nobody, adm and other</p>
<p>As we can see this users never log in the system – in scrin before:nologin and we have some list of them - we can distinguish them</p>
<p>2.Uid is unique identify number of the user/ Number can be consist of not more than 65535, usually it is positive number. Some number is reserved – 0 for root. 1-999 for special users (pseudo users, daemon and reserved users)</p>
<p>We can define id by tiping “id user”:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/2.1id.jpg)

<p>And in file /etc/passwd</p>

<p></p>
<p></p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m3/Task3.1/Scrin/2sqlconsole.jpg)

<p>3. GID – unique number for group. 0-for root, 1-99 for special users, 100+ for users</p>
<p>We can define them : id and /etc/passwd and /etc/group files</p>

<p>4. Specific group have specific number – until 1000 (99 the last number)</p>

<p>5. “useradd usersname” – we use  to create users. Basic parament that we need  its only login name. others are additional option   and if we didn’t write them we whould receive some by default (like group, uid, guid, shell)</p>

<p>6. sudo usermod -l newname oldname</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/6.1.jpg)

<p>7. skel-dir is used to initiate home directory when a user is first created, cotain information be default, have default Permission</p>
<p>We can see the example  /etc/skel:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/7.1.jpg)

<p>The default values for useradd in /etc/default/useradd:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/7.2defaultvalue.jpg)

<p>Permision for default /etc/skel – drwxr-xr-x – it’s not recommend to change. But we can change location for file or Home</p>

<p>8. userdel -r username – deleted the user’s home directory and mail spool.</p>

<p>9. We can locked users account in different way by using  passwd -l (u), usermod -lock (unlock), ‘chage’ command (modify user password expiration information) and others.</p>
<p>I used one of them:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/9.1.jpg)

<p>10. sudo passwd -d username– make a password-free </p>
<p>sudo passwd  -e username -  force user to change password</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/10.1.jpg)

<p>11.. /etc  It contains all system related configuration files in here or in its sub-directories; files, which can generally be edited by hand in a text editor. An l refers to a link that links to another file.</p>
<p>The first character include the type, next is permition strings ( some utribut can de changed on “-“ – It means that in this area we don’t have a permishin (read, wtite or use ). </p>
<p>Files and programs start with a hyphen (-). The last column : we have files - blue is a folder, white is a file,, green is a program or a binary </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/11.1.jpg)

<p>12. We have three level for permition: for user (the first three rwx), for groups (next three) and for others (the last three rwx). ALSO we can say in another way we have  the owner (user),  member of the group (group) and outsider (other)</p>
<p>About right:</p>
<p>r- it’s read</p>
<p>w- write</p>
<p>e- executeor we can say use</p>

<p>13. If users UID = files UID – it means, that user own this file. I f  the GID of the file the same as a group that user belong to? He is a member of the group. If we don’t find overlaps UID and GUID – we can  estimate user as outsider.</p>

<p>14. We can change the owner of file : </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/14.1.jpg)

<p>owner of group for dir and all of files within:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/14.2.jpg)

<p>Or change permition to file or dir by using chmod</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/14.3changeright.jpg)

<p>15.  we can to express rights by numbers. We know , that we have r=4, w=2, execute=1 – that means if we want give all the rights it should be 4+2+1=7 for u, 7 for g and 7 for o  ==777 – it’s for directory ,  and 666 for files (because without execute).</p>
<p>If we want give all rigts to some directory for u, r and w for group, and null for other  it will be 760, let’s check:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/15.1number.jpg)

<p>Umask – is a rights , that gives for default - the default file permission sets for newly created folders and files.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/15.2umaskS.jpg)

<p>We have umask 0002, and we can count and find out the permission:</p>
<p>777-0002 =775 =rwx (4+2+1) rwx re (4+1) – we can see this in our scrin after umask -S.</p>

<p>16. Sticky-bit is like protection from demage), in order to avoid deleting and ssecure your dir and files. We can set stiky bit in two ways – symbolic and numerical (by adding 1 before other permition, for example 1755). I set:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/16.1stickybit.jpg)

<p>And for deliting owner must : chmod o-t ~/test</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/16.2file.jpg)

<p>And come back without protection:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/16.3.jpg)

<p>17. If we want to execute this file -  attribute x should be present.</p>
<p>chmod ugo+x  filename</p>

<p>Thanks :)</p>

