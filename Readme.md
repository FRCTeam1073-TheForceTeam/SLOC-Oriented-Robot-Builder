SLOC Orientated Robot Builder
=============
This program is a modification of the code generating export functions from Brad Miller's and Alex Henning's FRC Code Template tool called Robot Builder. It can be found at http://firstforge.wpi.edu

This fork exists because the original program, while useful, generated way TOO many comments and other obstructions throughout my code. I generally do not care very much about SLOC or anything like that, but this just got too obnoxious. That said, the tool itself is pretty cool though.

Usage
-------
In `/dist/tools/` there is a jar called RobotBuilder.jar
Run that. By default, NetBeans will spit the compiled jar executable here after each build.

Main Diffrerences
-----------------
Comments still exist, but these are ones that I have deemed meaningful. If you disagree you can go fork this.

Supported Languages
-------------------
This modification provides support for less obnoxious Command Based Java and C++ code. 

Custom Headers
-------------
Additionally, the call to generate a header for a file is still in each template, however, the call ammends an empty String. This functionality exists so that you can flexibly add your own headers into the files that Robot Builder generates.

To modify the header macro, simply go into the appropriate macros.vm file for each language (Java or C++)
C++:	'/resources/export/cpp/macros.vm'
Java:	'/resources/export/java/macros.vm'
