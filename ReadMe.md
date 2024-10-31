# jdk8-demo-swingset2-redux ReadMe

`jdk8-demo:swingset2-redux` is a standalone update and reorganization of the `swingset2` demo(s) 
from the JDK samples[^1] for maven[^2], since they are still useful as a reference for using the various Swing package 
classes which are still available newer JDKs.

## Prerequistes

- JDK 8 or 9+ with the `java.desktop` module.

## Building with Maven
                    
Running maven's package plugin will complile a self-contained `swingset2-redux-VERSION.jar` file in the `target` directory.

### Pre-installed
                
Most Java development envronments will already have maven (`mvn`) avilable in the command line.

`mvn package`

### Wrapper Scripts

#### Unix(like) system shell

`./mvnw package`

#### Windows Command (batch) shell  

`mvnw.cmd package`

## Running

`java -jar target/swingset2-redux-VERSION.jar` 

## Modifications

### Build system

- Replaced `netbeans/ant` with 'maven'.
- Rearranged source and resources into Maven layout including a Project Object Model (`pom.xml`).
- Added Maven wrapper plugin[^3] scripts.

### Sources
          
Only minimal changes have been made to the original source as noted, leaving the original code and style in place
including static code warnings for serialization, non-final fields, etc.
     
#### [Deprecated Applet Removal](https://openjdk.org/jeps/289)

- Removed `SwingSet2Applet.java` and `SwingSet2.html` applet plugin HTML page.
- Removed `SwingSet2Applet` field, ctor arguments, getters, and checks from `SwingSet2.java`.

## Versions

- `1.0-SNAPSHOT` curent WIP.

## Files and Directories

- `artifacts` contains non-source related documentation located in the same path locations from the original `demo` directory.
- `artifacts/demo/java-dot-com-slash-bsd-license.txt`: text of the URL as referred to by `artifacts/demo/DEMOS_LICENSE`
- `artifacts/IntelliJ/runConfigurations`: IntelliJ IDE run configs.
- `src`: standard maven source and resources layout.

## References
  
[^1]: [Java SE Development Kit 8 Demos and Samples](https://www.oracle.com/java/technologies/java-archive-misc-downloads.html)
[^2]: [maven](https://maven.apache.org/)
[^3]: [Maven Wrapper](https://maven.apache.org/wrapper/index.html)