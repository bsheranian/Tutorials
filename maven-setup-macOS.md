Check if a jdk is already installed:
`java -version`

If nothing appears, download Java SE 8 here:
https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html

Check if JAVA_HOME is already set: 
`echo $JAVA_HOME`

If not set, export JAVA_HOME environment variable:
`echo export JAVA_HOME='/Library/Java/JavaVirtualMachines/jdk1.8.0_311.jdk/Contents/Home' >> ~/.bash_profile`

source ~/.bash_profile

test with `echo $JAVA_HOME`

Download binary zip archive of Maven:
https://maven.apache.org/download.cgi#

Set PATH environment variable:
`echo export PATH=/Users/sheranian/Developer/Maven/apache-maven-3.8.4/bin:$PATH >> ~/.bash_profile`

source ~/.bash_profile

Test with `mvn -version`

