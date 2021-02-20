
e.g. for Linux users with vscode.


1. download  jdk-15.0.2_linux-x64_bin.deb from https://www.oracle.com/java/technologies/javase-jdk15-downloads.html

2. install jdk-15.0.2_linux-x64_bin.deb 

3. cd  /usr/lib/jvm/jdk-15.0.2

4. sudo bin/jlink --module-path jmods --add-modules java.desktop --output jre

5. sudo vim ~/.bashrc
   export JAVA_HOME=/usr/lib/jvm/jdk-15.0.2

   export JRE_HOME=${JAVA_HOME}/jre

   export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib

   export PATH=${JAVA_HOME}/bin:$PATH

6. source ~/.bashrc

7. open vscode and install the floowing dependencies.

   Language Support for Java™ by Red Hat

   Debugger for Java

   Java Test Runner

   Maven for Java

   Java Dependency Viewer
   
   Project Manager for Java

   Java Extension Pack



8. enjoys