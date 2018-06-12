# RaspberryPi-MonitorTemp
MY IDEA:
I want to monitor temperature in server room with JianKongYi(www.jiankongyi.com) which has been deployed in DC.

On DTH11, from left to right, the pins is marked as 1, 2, 3 and 4.

I fix DTH11 with Pi, Pin1(VCC) connects to GPIO1 (BORAD), Pin2(DATA) connects to GPIO12, and Pin4(GND) conects to GPIO9.  

Write Python code(Python2) which can obtain temperature value and write into a log file.

Every 5 minutes, the porgram update once the status file(cur.txt) and append a line in log file(log.txt) as well.  In the information includes time, temperature, humity and status.

I also neet to install agent of "agent Linux" which is from JKY website in Pi.

JKY will fetch the key words in status file.  When JKY find keyword "Danger", it will alarm with message.
