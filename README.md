# djvu-html5
DjVu file viewer working as pure HTML5. Browse DjVu files without any additional tools or plugins!

Based on DjVu viewer implementation for Java by LizardTech, Inc.
http://sourceforge.net/projects/javadjvu/
Adapted and optimized for GWT framework (http://www.gwtproject.org/) by Mateusz Matela.
Released under the GNU General Public License version 2, see LICENSE file for details.

## Getting started

TBA

## Getting involved

The project is prepared with Eclipse and Google plugin. If you want another tool stack, you're on your own (feel free to other solutions once you figure them out).
1. Dwonload Eclipse from https://www.eclipse.org/downloads/, recommended package is IDE for Jave EE Developers.
2. Dwonload GWT SDK 2.7.0 from http://www.gwtproject.org/download.html
3. In Eclipse, go to `Help` -> `Install New Software...`, enter update site https://dl.google.com/eclipse/plugin/4.4 and select Google Plugin for Eclipse (version for 4.4 works with Eclipse 4.5). Install and restart.
4. In `Preferences` -> `Google` -> `Web Toolkit` provide the location where GWT SDK was unpacked.
5. Clone the GIT repository and import project `djvu-html5`.
6. There's an error in the project: The GWT SDK JAR gwt-servlet.jar is missing in the WEB-INF/lib directory.
In the Markers view, use a quick fix `The GWT SDK JAR gwt-servlet.jar is missing in the WEB-INF/lib directory`.
7. Right-click on the project, `Run as` -> `Web Application (GWT Super Dev Mode)`. The viewer should now be available here: http://127.0.0.1:8888/Djvu_html5.html
8. To prepare distribution that can be put on an external web server, right-click on the project, `Google` -> `GWT Compile`. Select the project and proceed with the compilation. Copy `djvu-html5/war` to the external server.
