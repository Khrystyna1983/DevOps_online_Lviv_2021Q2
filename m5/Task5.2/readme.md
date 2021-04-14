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

<p>3.GID – unique number for group. 0-for root, 1-99 for special users, 100+ for users</p>
<p>We can define them : id and /etc/passwd and /etc/group files</p>

<p>4. Specific group have specific number – until 1000 (99 the last number)</p>

<p>5. “useradd usersname” – we use  to create users. Basic parament that we need  its only login name. others are additional option   and if we didn’t write them we whould receive some by default (like group, uid, guid, shell)</p>

<p>6.sudo usermod -l newname oldname</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/6.1.jpg)

<p>7.skel-dir is used to initiate home directory when a user is first created, cotain information be default, have default Permission</p>
<p>We can see the example  /etc/skel:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/7.1.jpg)

<p>The default values for useradd in /etc/default/useradd:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/7.2defaultvalue.jpg)

<p>Permision for default /etc/skel – drwxr-xr-x – it’s not recommend to change. But we can change location for file or Home</p>

<p>8.userdel -r username – deleted the user’s home directory and mail spool.</p>

<p>9.We can locked users account in different way by using  passwd -l (u), usermod -lock (unlock), ‘chage’ command (modify user password expiration information) and others.</p>
<p>I used one of them:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/9.1.jpg)

<p>10. sudo passwd -d username– make a password-free </p>
<p>sudo passwd  -e username -  force user to change password</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.2/scrin/10.1.jpg)

<p>11.</p>

<p>12.</p>
<p></p>
<p></p>
<p></p>
