// To generate maven project(demo) from command line

-> mvn archetype : generate
-> Select 1808 (maven-archetype-quickstart)
-> Select version of quickstart from list of options(For now select 8)
-> Define value for property 'groupId' : com.telstra
-> Define value for property 'artifactId' : demo
-> Define value for property 'version' 1.0-SNAPSHOT : 1.0-SNAPSHOT
-> Define value for property 'package' :com.telstra.app
-> Select 'Y' for project build

-------------------------------------------------------------------------
Maven Lifecycle
-> mvn validate (If successful -> BUILD SUCCESS)
-> mvn compile (target directory created)
-> mvn test (If successful -> BUILD SUCCESS)
-> mvn package(generates the jar file after downloading the required plugins)
-> mvn verify (verifies the package, if successful -> BUILD SUCCESS)
-> mvn install (to install any package i.e. required)
==> It downloads all the plugins and information(local repository) in .m2 directory in C Drive for the corresponding project.

// Run Maven Application
(Using jar file)
-> java -cp demo-1.0-SNAPSHOT.jar com.telstra.app

