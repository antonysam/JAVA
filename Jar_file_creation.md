## Description of JAR file
```
JAR file stands for Java Archive. 

JAR file in java is a compressed version of the normal one.

The JAR file is used to store many types of files like audio file, video file, etc. 

This format is mainly used to distribute a set of Java classes. 

Using this, the downloading time decreased because of the small size of the file.

It can be executed from the java i.e., Java Web Start. 

To create the executable JAR file, you need to create a manifest file which is .mf file.
```
## Note
```
The JAR file format is based on zip format.

These types of files are mainly used for implementing libraries. 

Java Virtual Machine understands and implements these types of format for the java application.

To perform basic operations related to the JAR file, we use the Java Archive Tool (JAR tool). 

This tool is provided by the Java Development Kit (JDK)
```
## Creating a JAR File in Java
```
jar cf jarfilename inputfiles
//cf represents the creation of file.
C:\> jar cf pack.jar pack
```
## Viewing a JAR File in Java
```
jar tf jarfilename
// tf represents the contents of file
```
## Extracting 
```
jar xf jarfilename
//xf represents extracting of files
C:\> jar xf pack.jar
```
## Updating
```
jar uf jar-file input-file(s)
// updating the file
C:\>jar uf pack.ja
```
## Running 
```
C:\>java -jar pack.jar
```
