// To generate Maven Application using Eclipse

-> Select Maven Project from file tab.
-> Select maven-archetype-quickstart(version 1.4)
-> Provide groupId, artifactId,version,package.
-> Right click on project and run as maven build
   -> Setup the goals (apply from maven lifecycles)
       -> use either of the following
       -> validate
       -> compile 
       -> test 
       -> package
       -> verify  

// Can also run from command line


C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp>mvn validate
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------< com.telstra:demoApp >-------------------------
[INFO] Building demoApp 0.0.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  0.151 s
[INFO] Finished at: 2021-08-09T11:43:28+05:30
[INFO] ------------------------------------------------------------------------

C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp>mvn compile
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------< com.telstra:demoApp >-------------------------
[INFO] Building demoApp 0.0.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:3.0.2:resources (default-resources) @ demoApp ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\src\main\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.0:compile (default-compile) @ demoApp ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\target\classes
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  2.452 s
[INFO] Finished at: 2021-08-09T11:43:58+05:30
[INFO] ------------------------------------------------------------------------

C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp>mvn package
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------< com.telstra:demoApp >-------------------------
[INFO] Building demoApp 0.0.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:3.0.2:resources (default-resources) @ demoApp ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\src\main\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.0:compile (default-compile) @ demoApp ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:3.0.2:testResources (default-testResources) @ demoApp ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.0:testCompile (default-testCompile) @ demoApp ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\target\test-classes
[INFO]
[INFO] --- maven-surefire-plugin:2.22.1:test (default-test) @ demoApp ---
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.telstra.demoApp.AppTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.059 s - in com.telstra.demoApp.AppTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO]
[INFO] --- maven-jar-plugin:3.0.2:jar (default-jar) @ demoApp ---
[INFO] Building jar: C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp\target\demoApp-0.0.1-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  5.557 s
[INFO] Finished at: 2021-08-09T11:44:48+05:30
[INFO] ------------------------------------------------------------------------

C:\Users\d976996\OneDrive - Telstra\Documents\JFS\Day1\demoApp>
