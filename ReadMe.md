# jdk8-demo-swingset2-redux ReadMe

`jdk8-demo:swingset2-redux` is a standalone update and reorganization of the `swingset2` 
demo(s) from [Java SE Development Kit 8 Demos and Samples](https://www.oracle.com/java/technologies/java-archive-misc-downloads.html) for [maven](https://maven.apache.org/), since the examples
may still be useful with JDKs later than 8.

## Files and Directories

 - `artifacts` contains non-source related documentation located in the same path locations from the original `demo` directory.
 - `artifacts/demo/java-dot-com-slash-bsd-license.txt`: text of the URL as referred to by `artifacts/demo/DEMOS_LICENSE`
 - `artifacts/IntelliJ/runConfigurations`: IntelliJ IDE run configs.
 - `src`: standard maven source and resources layout.

## Building

`mvn package` compiles and packages a selfcontained jar file, `target/swingset2-redux-VERSION.jar`
 
## Running

`java -jar target/swingset2-redux-VERSION.jar` 

## Modifications

### Build system

- Replaced `netbeans/ant` with 'maven'.
- Rearranged source and resources into maven layout.

### Sources
          
Only minimal changes have been made to the original source as noted, leaving the original code and style in place
including static code warnings for serialization, non-final fields, etc.
     
#### [Deprecated Applet Removal](https://openjdk.org/jeps/289)

- Removed `SwingSet2Applet.java` and `SwingSet2.html` applet plugin HTML page.
- Removed `SwingSet2Applet` field, ctor arguments, getters, and checks from `SwingSet2.java`.

## Versions

- `1.0-SNAPSHOT` curent WIP.