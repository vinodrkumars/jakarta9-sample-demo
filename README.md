# jakarta9-sample-demo

## Creating project from mvn command - 


Creating JakartaEE 9 project 

```
mvn -B  archetype:generate \
-DarchetypeGroupId=io.github.hantsy \
-DarchetypeArtifactId=maven-archetype-jakartaee9  \
-DarchetypeVersion=1.0  \
-DgroupId=com.demo \
-Dpackage=com.demo \
-DartifactId=Jakarta9-sample-demo \
-Dversion=1.0-SNAPSHOT
```

## Running project - 

```

$ mvn -X clean package cargo:run
Apache Maven 3.6.3 (cecedd343002696d0abb50b32b541b8a6ba2883f)
Maven home: /Users/Shared/tools/apache-maven-3.6.3
Java version: 11.0.6, vendor: AdoptOpenJDK, runtime: /Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x", version: "10.16", arch: "x86_64", family: "mac"
.......
.......

[DEBUG] [URLDeployableMonitor] Notifying monitor listener [org.codehaus.cargo.container.spi.deployer.DeployerWatchdog@65ad2b42]
[INFO] [talledLocalContainer] GlassFish 6.1.0 started on port [8080]

[INFO] Press Ctrl-C to stop the container...

^C[INFO] [talledLocalContainer] GlassFish 6.1.0 is stopping...


```

Testing URL 
http://localhost:8080/Jakarta9-sample-demo/api/greeting/<greetingMessage>



