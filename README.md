
# trsm
Tomcat Redis cluster Session Manager

1.Add content to  tomcat context.xml 

Valve className="cn.inps.trsm.RedisSessionHandlerValve" 
Manager className="cn.inps.trsm.RedisSessionManager" hosts="10.245.5.80:7000,10.245.5.80:7001,10.245.5.80:7002" maxInactiveInterval="60"

2.Add jar file to Tomcat

copy commons-pool2-2.4.2.jar
jedis-2.8.2.jar
tomcat-juli-7.0.27.jar 
trsm.jar  to 
/usr/local/tomcat/lib/ 
