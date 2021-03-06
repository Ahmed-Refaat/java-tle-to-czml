# java-tle-to-czml #

### Description ###

* A library to create CZML for satellites. Can also be used as a java library for other applications or to extend!
* 1.0
* Author:
	Ryan Pelletier
	
![Imgur](https://i.imgur.com/vZLc6qF.png)

## How To ##

### Use ###
Run the jar in the same directory as your tles.txt file. An example tles.txt is in the root of this project, you can use multiple TLEs.
```bash
java -jar java-tle-to-czml-1.0-RELEASE.jar
```
Use the output satellites.czml file in Cesium. You can easily to this with [Cesium Sandcastle](https://cesiumjs.org/Cesium/Build/Apps/Sandcastle/#c=bZBLT8MwEIT/ismlQUK2ODetkMIRCaQiTr449pauurYjP1I1vx4n4VEoN+/MfLNaC9HnxNIBmPYugUuR+T2LKgERJohcj5YYuiUyvQcVUHUETDnDQnY30hVp8TZsLd0yDwgnCEVxcGItRMyWv81avdLz2JaFCh2E1e16YYxKaudz0PASvMUIBf9E21L/+G1z8srU08oZnWv5Dx25Mqa+arvIjt7bV/9/pLqrmpjOBFvpHtD2PiSWA9WciwS2p/I3UXRZHyFxHeOENOILaAwODM1GVn+OlBXTpGIszj4T7XAEWW0bUfK/sOkydO/PAwRS5ylyuN8+LSLnvBFlvKaS99SpcNEo3Qc)

### Develop ###
```bash
git clone https://github.com/ryanp102694/java-tle-to-czml.git
cd java-tle-to-czml
```
 *If you develop locally you need to install these jars from the project's lib directory into your local maven repo*
 ```bash
mvn install:install-file -Dfile=${basedir}\lib\cesiumlanguagewriter-2.10.0.jar -DgroupId=agi.foundation -DartifactId=cesiumlanguagewriter -Dversion=2.10.0 -Dpackaging=jar
mvn install:install-file -Dfile=${basedir}\lib\math-1.0-SNAPSHOT.jar -DgroupId=gov.sandia.phoenix -DartifactId=math -Dversion=1.0 -Dpackaging=jar
mvn install:install-file -Dfile=${basedir}\lib\astrodynamics-1.0-SNAPSHOT.jar -DgroupId=gov.sandia.phoenix -DartifactId=astrodynamics -Dversion=1.0 -Dpackaging=jar
```
In order to build the jar run
```bash
mvn clean package
```
