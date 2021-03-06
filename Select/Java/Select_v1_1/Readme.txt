		Generation & Build of Vindicia Select v1.1 Java Library
		-------------------------------------------------------

Files:

	Select_wsdl2java.sh		- Generates Java source files from Select WSDL
	Select_wsdl2java.bat	- Generates Java source files from Select WSDL (Windows)
	build.sh				- Compiles source, creates VindiciaSelect_v1_1.jar & javadocs
	build.bat				- Compiles source, creates VindiciaSelect_v1_1.jar & javadocs (Windows)
	build.xml				- Project file generated from wsdl2java, uses Ant instead of .sh/.bat
	docs					- Javadocs for source files generated from Select WSDL
	src						- Java source files generated from Select WSDL (+mod to ReturnCode.java)
	test					- Java test source files generated from Select WSDL
	wsdls					- Local copies of Select WSDL files (+mod to swap order of Return Type)
	Readme.txt				- This file (Start Here)

	howto_convert_wsdls_to_local_and_generate_java_stubs.txt	- Detailed steps to generate Library
	Issues_&_Resolution_Select_library_generation.txt			- 2 Issues in build & resolutions



Installation
------------

0. Choose working directory, referenced as <Base Path> below.

1. Install Axis2 1.6.2 binary distribution to obtain Axis jar files from:

	http://axis.apache.org/axis2/java/core/download.cgi

   Extract axis2-1.6.2-bin.zip (or Axis2.zip) so it is populated in the directory:

	<Base Path>/Axis2/axis2-1.6.2

The above is required to either build with the jar file or generate from source
& build the the jar file for either the binary or source distribution in the
steps below:


2. For the binary version of this distribution:

	Obtain the jar file, VindiciaSelect_v1_1.jar & include it in your ClassPath
	of your example Project which makes calls to the Select v1.1 API.
   
   Binary version is on GitHub in Releases at:
   
		https://github.com/Vindicia/CashBoxAPISamples/releases/Select_v1_1
		https://github.com/Vindicia/CashBoxAPISamples/files/124097/Select_v1_1.zip
   
3. If you wish to generate Java source files from the Select WSDL, and
   compile source to generate the jar file for the Select v1.1 API:
   
	Follow the steps outlined in the text file describing Detailed steps
	to generate Library listed Files above, making the 2 modifications
	as described there.
   
   Source distribution is on GitHub at:
   
		https://github.com/Vindicia/CashBoxAPISamples/tree/master/Select/Java/Select_v1_1

