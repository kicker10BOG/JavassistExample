# Javassist Example
This code is slightly modified from javapapers.com/core-java/java-instrumentation/ which is
a very good example of how to start using Javassist. 

### To compile
* In Eclipse, use right-click the "example.jardesc" file and click "Create Jar"
* From command line:
  1. Navigate to the "bin" directory
  2. Type: `jar cvfm example.jar ..\META-INF\MANIFEST.MF .` 

### To Run
From the command line, type: 
```
java -cp .;.\javassist.jar -javaagent:.\example.jar javassistExample.TestInstrumentation
```