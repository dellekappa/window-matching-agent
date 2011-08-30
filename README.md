Window Matching Agent
=====================

The Window Matching Agent is a simple java agent that uses bytecode manipulation to change the value
sun.awt.X11.XToolkit assigns to the WM_CLASS property

Building from source
--------------------

Make sure you have have [maven](http://maven.apache.org) installed then from the commandline run :

mvn package

the generated agent.jar file will end up in the target folder

Downloading binaries
--------------------

You can download a [recent binary](http://jelmer.s3.amazonaws.com/agent.jar) from amazon s3

Usage
-----

To use it add the following argument to your commandline

-javaagent:agent.jar=YOUR_APPLICATION_IDENTIFIER

and assure that asm v3.3.1 is in the classpath
