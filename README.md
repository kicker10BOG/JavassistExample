# Javassist Example
This code is slightly modified from [javapapers.com/core-java/java-instrumentation/](javapapers.com/core-java/java-instrumentation/) which is
a very good example of how to start using Javassist. 

Clearly, since this is a Javassist tutorial, you need to have the 
[Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) 
installed and the 
[Javassist library](http://jboss-javassist.github.io/javassist/) 
somewhere on your computer. 

### To compile
* In Eclipse, right-click the "example.jardesc" file and click "Create Jar"
* From command line:
  1. Navigate to the "bin" directory
  2. Type: `jar cvfm example.jar ..\META-INF\MANIFEST.MF .` 

### To Run
From the command line in the "bin" directory, type: 
```
java -cp .;..\..\lib\javassist.jar -javaagent:.\example.jar javassistExample.TestInstrumentation
```
Note: Replace `..\..\lib\javassist.jar` with the path to Javassist on your computer. 