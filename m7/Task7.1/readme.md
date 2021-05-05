<h2>B</h2>
<p>1. From which ip were the most requests?</p>
<p>We neded 2 files – 1- our bash -script, and 2- our apache_logs</p>
<p>Create the script and run:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/1.1.jpg)

<p> Where grep -E -o – extended regular expression, -o print only non-empty parts of maching line , each part consider as separate output line</p>
<p>$1- argument 1 </p>
<p>Sort -sort lines</p>
<p>uniq -c – count  uniq numbers</p>
<p>sort gr – find out most requested id – sort by the most  requested in file_out( apache_logs)</p>
<p>read line1-we read each string  from file_out</p>
<p>and echo which ip were the most requested (we have seen in scrin before)</p>

<h3>2. What is the most requested page?</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B2.1.jpg)


<h3>3.How many requests were there from each ip?</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B3.2.jpg)

<p>Or we can use command in command line:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B3.1.jpg)

<h3>4. What non-existent pages were clients referred to?</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B4.3.jpg)

<p>You also can search 404error in all documents</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B4.1.jpg)

<p>Or only count the number:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B4.2.jpg)


<h3>5. What time did site get the most requests?</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/В5.2.jpg)

<p>If we talk only about Hours and minutes it’s :</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/B5.1.jpg)


<h3>6.  We can find out about bots or suspect them , when:</h3>
<p>- we have bulb request (in 6th column)  </p>
<p>-  have status 403 in 9 column</p>
<p>- we can analyze from which browser  came request </p>
<p>- use different  extra utilits</p>
<p>We can use bush-script with popular list of bots  in order to find them:</p>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/6.1.jpg)



<h3>***</h3>
<h3>I created additional script for practice:</h3>

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/1.2.jpg)

![](https://github.com/Khrystyna1983/DevOps_online_Lviv_2021Q2/raw/master/m7/Task7.1/Scrin/1.1.jpg)




<p>Thank you :)</p>
