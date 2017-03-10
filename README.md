This is a demo webapp based on:
https://www.tutorialspoint.com/maven/maven_web_application.htm

The purpose is:
- Additional experience with maven (I'm using maven since 2014, but the possibilities never cease to amaze me).
- Create a little demo web app to show how to create this, using a built-in tomcat web server.
  This is handy if you would like to study somewhere but you don't want to install tomcat wherever you work / study.
  
How to run this application:

	$ mvn clean install
	or
	$ mvn clean package

	$ mvn tomcat7:run

The startup logging:
	[INFO] Scanning for projects...
	[INFO]
	[INFO] ------------------------------------------------------------------------
	[INFO] Building trucks Maven Webapp 1.0-SNAPSHOT
	[INFO] ------------------------------------------------------------------------
	[INFO]
	[INFO] >>> tomcat7-maven-plugin:2.2:run (default-cli) > process-classes @ trucks >>>
	[INFO]
	[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ trucks ---
	[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
	[INFO] Copying 0 resource
	[INFO]
	[INFO] --- maven-compiler-plugin:3.6.0:compile (default-compile) @ trucks ---
	[INFO] No sources to compile
	[INFO]
	[INFO] <<< tomcat7-maven-plugin:2.2:run (default-cli) < process-classes @ trucks <<<
	[INFO]
	[INFO] --- tomcat7-maven-plugin:2.2:run (default-cli) @ trucks ---
	[INFO] Running war on http://localhost:8899/trucks					----> Configured in pom.xml !!!
	[INFO] Creating Tomcat server configuration at D:\Java\Studie\maven\tutorialspointworkspace\trucks\target\tomcat
	[INFO] create webapp with contextPath: /trucks
	Mar 02, 2017 3:01:39 PM org.apache.coyote.AbstractProtocol init
	INFO: Initializing ProtocolHandler ["http-bio-8899"]
	Mar 02, 2017 3:01:39 PM org.apache.catalina.core.StandardService startInternal
	INFO: Starting service Tomcat
	Mar 02, 2017 3:01:39 PM org.apache.catalina.core.StandardEngine startInternal
	INFO: Starting Servlet Engine: Apache Tomcat/7.0.47
	Mar 02, 2017 3:01:41 PM org.apache.coyote.AbstractProtocol start
	INFO: Starting ProtocolHandler ["http-bio-8899"]

How to reach the web site:
	http://localhost:8899/trucks/index.jsp

