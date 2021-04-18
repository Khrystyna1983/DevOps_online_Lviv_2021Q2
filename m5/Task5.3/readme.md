<h2>Task 5.3</h2>
<h3>PART 1</h3>
<p>1.	We have two fundamental types of processes: foreground and background. If we talk about states, there are 5: created, ready, running, terminate, waiting</p>
<p>2.	Pstree shows us  running processes in a tree (data structure).</p>
<p>pstree -p -show a tree with their PIDs</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/2.1pstree.jpg)

<p>pstree -p kh (username) - to display all process trees rooted at processes owned by a specific user with their PIDs</p>
<p>pstree -np - to sort processes by PID instead of by name</p>
<p> pstree -l - to wrap long lines</p>
<p>we have a lot of other options, for example </p>
<p>-g Show PGIDs</p>
<p>-n Sort processes with the same parent by PID instead of by name and so on</p>
<p>Highlight the current process and its ancestors we can get by typing: pstree -h </p>

<p>3.	The directory /proc contains (among other things) one subdirectory for each process running on the system, which is named after the process ID (PID).  It’s specific file. Each process subdirectory has the entries listed and responsible for same of important part of processes.</p>
<p>exe - Link to the executable of this process, fd - directory, which contains all file descriptors, cpu -current and last cpu in which it was executed and so on </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/3.1.jpg)

<p>For example, to get the status information of a process, all you have to do is read the file /proc/PID/status:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/3.2pros.jpg)

<p>/proc/meminfo - Provides information about distribution and utilization of memory. This varies by architecture and compile options.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/3.3meminfo.jpg)

<p>and others processes</p>
<p>We can find out a lot of information from this file.</p>

<p>4. less /proc/cpuinfo</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/4.1cpuinfo.jpg)

<p>5. We can use ps -eF  or ps  -efl for this aim: </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/5.1.jpg)

<p>6.	Kernel threads are in square brackets. We can’t manage them or kill, each of Kernel process is started with its own process identification number (PID).</p>

<p>7.	If we type ps aux – we can see a snapshot with prosesses and their status:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/7.1psaux.jpg)

<p>Ss – means  interruptible sleep (waiting for an event to complete) or we can sad sleeping and  s- is a session leader</p>
<p>I< - swapped out process with high priority</p>
<p>R - running or runable</p>
<p>Some of them are stable, state , same of them can be started when some clause will happend, processes with  state “R” are working. If we want to see only active proceses  should type: ps -A or ps -e</p>
<p>We can see a real information of processes by typing  top command :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/7.2.jpg)


<p>8.	For  a specific user we can manage :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/8.1.jpg)

<p>Or ps -u admin(username)</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/8.2psfu.jpg)


<p>9.	Ps T   shows process accotiated to terminal (this terminal)</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/9.1.jpg)

<p>Find out about high occupied memory process:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/9.2.jpg)

<p>ps -A or ps -e shows all started processes</p>
<p>ps -d all session without leaders</p>
<p>ps -r all running process </p>
<p>Ps -e, -ef, -ely – every process</p>
<p>Ps -elf, axmy  -info abaut thread</p>
<p>Ps -x – process that have tty</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/9.3.jpg)


<p>10.	Top  give us information about system, how loaded our system is</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/10.1.jpg)

<p>Before table we see total information:</p>
<p>Before table we see total information:
current time, up – how long the system is working,  user – current users, load average – loaded system 1 min befor, next -5, and 15. This number should be more then count of existing core in system
</p>
<p>The next line  - info about task and their status and next - info about the state of processor</p>
<p>In the table:</p>
<p>PID – unique process id.</p>
<p>User -who run this process</p>
<p>Pr we can see priority, </p>
<p>NI – priority by nice</p>
<p>VIRT – total virtual memory used by the task</p>
<p>RES – physical memory occupying a process, </p>
<p>SHR –main memore that engaged  with sharing from other. </p>
<p>S -current status</p>
<p>CPU - % , ercentage of the main dimensions of the central processor, </p>
<p>%Mem - Shows the Memory usage of task.</p>
<p>TIME+ - how long process is starting, </p>
<p>COMMAND – command that initiated a process</p>

<p>11.	Top -u  username</p>
<p>We can Press ‘c‘ option in running top command, also we can sort information  in different way by using hot key</p>

<p>12.	Pressed ‘c‘ option in running top command- it displays absolute path of running process</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/12.1top.jpg)

<p>We can find the proceses of some user – press u and type username </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/12.2.jpg)

<p>Killed  prosess- press k and type PID</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/12.3.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/12.4.jpg)

<p>WE can use ‘r‘ option to change the priority of the process also called Renice and other option</p>

<p>13. Shift +t  - sorted by running time</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/13.1.jpg)

<p>Ctrl Z – stoped top</p>
<p>Fg -resume</p>
<p>Shift+t -show information about CPU state</p>
<p>Shift+m -memory usage</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/13.2m.jpg)


<p>14. </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/14.1.jpg)

<p>15. To set priority we can use renice  in top - to change the niceness priority</p>
<p>Press r , type PID and type value</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/15.1.jpg)

<p>16.Lets start processes sleep. We can kill the process by using kill and type PID of process: </p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/16.1.jpg)

<p>If we want kill all the processes @sleep we should type  - “kill all sleep” – but in this case we killed all our process. Onle for current user – if we want kill all the users processes we shoud do this as a root.</p>
<p>There is one more command to kill the prosses – is pkill – but we should type  +name of process, that can be not so convenient.</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/16.2.jpg)

<p>The various integers, and the symbolic name they are mapped to, can be listed using the kill -l:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/16.3.jpg)

<p>For example I used Sighkill – is a signal to stop process execute immidiatly. Program can’t ignore this</p>
<p>Kill SIGKILL PID  or kill -9 PID:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/16.4.jpg)


<p>17.  fg – type of processes, that execute when we cooperate with terminal session. We type the command -  fg do it. We can do something else by ignoring this process.
  Bg – is a process that can be executed without connection to a terminal, it don’t expect command or cooperation
</p>
<p>When we finished the session – all  fg and bg processes have been stopped. In this case we can use  and set nohup process  - to continuose work without active session.</p>
<p>Jobs shows us  the processes. It’s command for the ability to stop/suspend the execution of processes, and continue/resume their execution as per your requirements</p>
<p>If we run command sleep in fg we can’t do some another command :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/17.1.jpg)

<p>We should press ctrl+c to exit</p>
<p>We can run  bg process (by using & at the end):</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/17.2.jpg)

<p>And my work with yes :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m5/Task5.3/Scrin1/17.3.jpg)


<h3>PART 2</h3>

<p></p>
<p></p>
<p></p>
<p></p>


<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
<p></p>
