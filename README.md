# RaspberryPi-MonitorTemp
MY IDEA:
I want to monitor temperature in server room with JianKongYi(www.jiankongyi.com) which has been deployed in DC.

I fix DTH11 with Pi, Pin1 connects to GPIO1 (BORAD), Pin2 connects to GPIO12, and Pin4 conects to GPIO9.  

Write Python code(Python2) which can obtain temperature value and write into a log file.

Every 5 minutes, the porgram update once the status file(cur.txt) and append a line in log file(log.txt) as well.  In the information includes time, temperature, humity and status.

I also neet to install agent of "agent Linux" which is from JKY in Pi.

JKY will fetch the key words in log file.  When JKY find "Danger", it will alarm with message.
