

# trsm
Tomcat Redis cluster Session Manager support to store session using Redis cluster 


1.Add content to  tomcat context.xml 

Valve className="cn.inps.trsm.RedisSessionHandlerValve"

Manager className="cn.inps.trsm.RedisSessionManager" hosts="10.172.2.50:7000,10.172.2.50:7001,10.172.2.50:7002,10.172.2.50:7003" maxInactiveInterval="60"

2.Add jar file to Tomcat

copy commons-pool2-2.4.2.jar
jedis-2.8.2.jar
tomcat-juli-7.0.27.jar 
trsm.jar  to 
/usr/local/tomcat/lib/ 
