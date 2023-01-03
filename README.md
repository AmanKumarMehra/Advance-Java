# Advance-Java

## JVM
JVM(Java Virtual Machine) acts as a run-time engine to run Java applications. JVM is the one that actually calls the main method present in a java code. JVM is a part of JRE(Java Runtime Environment).

### JVM consists of 
- Class Loader - Loading, Linking, Initailisation.
- JVM Memory - Method Area, Heap Area, Stack Area, PC register, Native method area.

### Class Loader consists of 
1) Loding - Bootstrap class loader, Extension class loader, Application class loader
- Bootstrap Class Loader – It loads JDK internal classes. It loads rt.jar and other core classes for example java.lang.* package classes.
- Extensions Class Loader – It loads classes from the JDK extensions directory, usually $JAVA_HOME/lib/ext directory.
- System Class Loader – This classloader loads classes from the current classpath. We can set classpath while invoking a program using -cp or -classpath command line option.
          
2) Linking - Verification, Preparation, Resolution
- Verification - Verify the bytecode, which makes java secure.
- Preparation - Allocate memory to class level data, like it initialise static variable with value 0.
- Resolution - Replace symbolic name with actual name.

3) Initalisation-
- All static variables are assigned with original value.
- Static block will be executed from top to bottom.

## Thread
### We can create Threads in java using two ways, namely : 
- By extending Thread Class
- By Implementing a Runnable interface

