# MobileFirst Cordova Labs Prerequisites

> **IMPORTANT:** This series of labs assumes you are using a **Mac** with the **macOS operating system**. If you are using Windows or Linux you will need to ensure that you have also installed and properly configured the Anddroid Studio.

Generally speaking it is recommended that you install the latest versions of the software listed. If you have older installations please ensure that you have upgraded to the currently recommended versions.

## Prerequisites
To run the labs you will need to have the following tools installed on your laptop computer. You can install natively or create a virtual machine if you desire.

The required tools to install include:

- Install Java
- Install NodeJS
- Install Cordova
- Install Ionic Command-Line-Utility
- install gulp
- Install Maven
- Install MobileFirst 8.0 Command Line Utility
- Install MobileFirst 8.0 Development Kit
- Install IntelliJ IDEA Community Edition
- Install Brackets

Optional installs

- Create Bluemix Account
- Create an Ionic Creator Account
- Android Studio (for Windows and Linux users)

## Install Java
You will need one of the following installed:
- Oracle JVM 1.7u55+
- Oracle JVM 1.8u20+
- IcedTea OpenJDK 1.7.0.55+

To Install Oracle Java on a Mac or Windows Machine visit http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html. The current version as of the April 11, 2016 is 8u77.

Download from the section that reads: Java SE Development Kit 8u77. Accept the License Agreement to enable the selection and download of the appropriate installation.

To install IcedTea OpenJDK on a Debian, Ubuntu, Fedora, Oracle Linux or Red Hat Linux machine visit http://openjdk.java.net/install/index.html and follow the instructions to download and install.

## Install NodeJS
There are two current stable builds of NodeJS as of 4/11/2016. Download and install version 4.4.2 or the Stable LTS version. We do not recommend installing 5.10.1

Visit `https://nodejs.org/en/download/` and download the version that matches your operating system. 

### Confirm installation
After the install you will want to confirm that the installation was successful. **On Mac or Linux** open a terminal or **On Windows** open a command prompt and type `node -v`.

## Install Cordova
Once node is installed you can use npm to install Cordova. The current version as of 4/11/2016 is 6.1.1

1. To determine your version of Cordova if you have one previously installed open a command prompt (Windows) or terminal (Mac/Linux) and type `cordova -v`.

1. To install Cordova if it is not currently installed or is a later version:

	**On Mac or Linux** open a terminal and type:

	`sudo npm install -g cordova`

	**On Windows** open a command prompt and type:

	`npm install -g cordova`

1. Confirm the correct version by typing `cordova -v`


## Install Ionic Command-Line-Utility
You will need the Ionic Command-Line-Utility to complete the labs. To install the Ionic Command-Line-Utility you will again use npm. As of 4/11/2016 the current version of Ionic is 1.7.14

1. To install Ionic if it is not currently installed or is a later version:

	**On Mac or Linux** open a terminal and type:

	`sudo npm install -g ionic`

	**On Windows** open a command prompt and type:

	`npm install -g ionic`

1. Confirm the correct version by typing `ionic -v`

## Install Gulp

```
npm install -g gulp```
```

## Install Maven
The current version of Maven as of 4/11/2016 is 3.3.9. For more information on installing Maven, please visit https://maven.apache.org/install.html

1. Download the Maven binary `apache-maven-3.3.9-bin.tar.gz` or `apache-maven-3.3.9-bin.zip` from https://maven.apache.org/download.cgi

1. Unpack the tar or zip file.

### For Mac
1. Move the contents of the upacked directory. Open a terminal and type:

	`mv /Users/[myuser]/Downloads/apach-maven* /opt/`
	
	Replacing the `[myuser]` with your computer user name.

1. Edit your .profile to add the location of maven to your path. Open a terminal and type:

	`pico $HOME/.profile`
	
1. Enter the following on a new line or update your existing path statement:
	`export PATH=$PATH:/opt/apache-maven-3.3.9/bin`
	
1.	Ctrl-O to write the file

1.	Ctrl-X to exit pico editor

1.	Make the path available. Type

	`source $HOME/.profile`
	
	This will run the profile and make the new path available.
	
1. Verify the installtion. Type

	`mvn -v`
	
	This should return something like
	
	```
	Apache Maven 3.3.9 (bb52d8502b132ec0a5a3f4c09453c07478323dc5; 2015-11-10T08:41:47-08:00)
Maven home: /opt/apache-maven-3.3.9
Java version: 1.8.0_60, vendor: Oracle Corporation
Java home: /Library/Java/JavaVirtualMachines/jdk1.8.0_60.jdk/Contents/Home/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x", version: "10.11.4", arch: "x86_64", family: "mac"
```

### For Windows
1. Instead of re-writing the example of how to install Maven on Windows, follow this tutorial: http://www.mkyong.com/maven/how-to-install-maven-in-windows/

> Note that since you have already installed Java, you can skip that portion of the tutorial on mkyong.com.

## Install MobileFirst 8.0 Command Line Utility

The development version of the MobileFirst Command Line Utility is now available as an npm install. This version can coexist with previous versions of the MobileFirst Command Line Utility.

To install the MobileFirst CLI Version 8.0 Beta, open a terminal or command prompt and type 

```npm install -g mfpdev-cli```

You can confirm the installation by typing

```mfpdev -v```

You should see something similar to

`8.0.0-XXXXXXXXXXXX`

## Install MobileFirst 8.0 Development Kit
IBM MobileFirst Platform Foundation v8.0 beta consists of the following components: MobileFirst Server & MobileFirst Operations Console, MobileFirst Command-line Interface (CLI), MobileFirst client SDKs and MobileFirst adapter tooling.

These components can be installed either seperately via online repositories which contain the latest releases, or downloaded bundled together through the MobileFirst Platform Foundation Development Kit Installer, for future or offline use.

> **Note:** That you installed the CLI (Command-Line-Interface) from npm in the previous step. 

## Install IntelliJ IDEA Community Edition
For the labs you will need an editor, preferably one that supports Java, Maven, and Git. We have chosen IntelliJ Community Edition because it supports all the features we need to run the labs.

To install IntelliJ, visit https://www.jetbrains.com/idea/download/ and select the operating system you are running (Mac, Windows, or Linux) and download. Run the appropriate installation from the download.

## Create a Bluemix Account
Please ensure that you have created a Bluemix account and that you can log into it. If you have not created a Bluemix account please do so using your IBM id at https://console.ng.bluemix.net/registration/

A Bluemix account is required to complete the installation instructions as well as the labs.

## Create an Ionic Creator Account (Optional)
If you would like to have a tool for visually creating your Ionic User interface, then you may want to create an account at Ionic Creator. To do that visit https://creator.ionic.io/app/signup and signup.

> **Note:** None of the labs require Ionic Creator so it is not mandatory

## Important Links
[Java Download](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

[NodeJS Download](https://nodejs.org/en/download/)

[NodeJS Documentation](https://nodejs.org/dist/latest-v4.x/docs/api/)

[Cordova Home](https://cordova.apache.org)

[Ionic Home](http://ionicframework.com)

[Ionic Documentation](http://ionicframework.com/docs/)

[Maven Home](https://maven.apache.org)

[Maven Documentation](https://maven.apache.org/guides/index.html)

[Bluemix](https://console.ng.bluemix.net)

[Mobile Foundation on Bluemix Documentation](https://console.ng.bluemix.net/docs/services/mobilefoundation/index.html)

[IBM MobileFirst Home](https://mobilefirstplatform.ibmcloud.com/)

[IBM MobileFirst 8.0 Downloads](https://mobilefirstplatform.ibmcloud.com/downloads/)

[IBM MobileFirst 8.0 Documentation](http://www.ibm.com/support/knowledgecenter/SSHS8R_8.0.0/wl_welcome.html?cp=SSVNYL)

[IntelliJ IDEA Home](https://www.jetbrains.com/idea/)


