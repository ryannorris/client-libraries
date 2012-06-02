CarePass Java Client Libraries
=============================

The goal of these libraries is to remove the need for a CarePass developer to manage the baseline connectivity and data un-packing of interacting with the CarePass APIs.

About CarePass APIs
===================
Read all about the available API's at http://developer.carepass.com

Quick Start: Examples you can use
=================================
For the best example as to how to use the iOS library for the CarePass APIs, view the unit tests.

To use the library asynchronously (recommended for mobile applications), you would need to set the delegate on each request that will handle when the response returns. See the sample iOS app <https://github.com/carepass/code-samples> for an example of this implementation pattern.

Adding the CarePass Java Client Libraries to Your Project
========================================================

The Java Client library for CarePass is a Maven project.  While it is not available in a Maven repository, you may download it and build it locally.  It will load it's own dependencies from external repositories.

1.  The code for the project can be found here:  <https://github.com/carepass/client-libraries/tree/Java>
2.  If you do not already have Maven installed, it can be downloaded here: <http://maven.apache.org/download.html>
3.  Once you have downloaded the code and installed Maven, build the project by using `mvn clean install`

You can then add the built project to your own maven project with the below dependency:

	<dependency>
		<groupId>com.aetna.carepass</groupId>
		<artifactId>carepass-api</artifactId>
	</dependency>
	
For an example of how to use the API, including key configuration, see `/carepass-api/src/main/java/com/aetna/carepass/CarePassApplication.java` in the source
