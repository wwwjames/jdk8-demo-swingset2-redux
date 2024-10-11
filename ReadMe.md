# jdk8-demo-swingset2-redux ReadMe

`jdk8-demo:swingset2-redux` is a stand alone repackaging of the `swingset2` demo from [Java SE Development Kit 8 Demos and Samples](https://www.oracle.com/java/technologies/java-archive-misc-downloads.html),
which is built with `maven` instead of [NetBeans](https://netbeans.apache.org/front/main/index.html), and has been rearranged to conform to `maven` source and resource layout conventions.


## Files and Directories

 - `artifacts` contains non-source related documentation located in the same path locations from the original `demo` directory.
 - `artifacts/demo/java-dot-com-slash-bsd-license.txt`: text of the URL as referred to by `artifacts/demo/DEMOS_LICENSE`
 - `artifacts/IntelliJ/runConfigurations`: IntelliJ IDE run configs.
 - `src`: standard maven source and resources layout.


## Building

`mvn package` compiles and packages a selfcontained jar file, `target/swingset2-redux-VERSION.jar`
 
## Running

`java -jar target/swingset2-redux-VERSION.jar` 
