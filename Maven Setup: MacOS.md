# Setting Up Maven: MacOS

## Requirements:
* 10MB of space for Maven installation
* 500MB of space for Maven's repo


### Check if a JDK is already installed

`java -version`

(Must be 1.7 or later)

If nothing appears, download and install the [Java SE 8 JDK](https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html) from Oracle

### Check if JAVA_HOME is already set:

`echo $JAVA_HOME`

If not set, export JAVA_HOME environment variable with
`echo export "JAVA_HOME=\$(/usr/libexec/java_home -v 1.8.0)" >> ~/.bash_profile`

Update your instance of bash with
`source ~/.bash_profile`

test with
`echo $JAVA_HOME`

### Download Maven

Download a *binary zip archive* of [Apache Maven](https://maven.apache.org/download.cgi#)

Unzip the archive in a folder of your choosing with 
`unzip apache-maven-3.8.4-bin.zip`

Set PATH environment variable with
`echo export PATH=DIRECTORY/apache-maven-3.8.4/bin:$PATH >> ~/.bash_profile`
, replacing "DIRECTORY" with the absolute path to the folder you chose to unzip your archive in.

Update your instance of bash with
`source ~/.bash_profile`

Test with
`mvn -version`

### Done!

