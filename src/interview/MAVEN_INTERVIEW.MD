# Maven Interview Questions

* What is the difference between Maven dependency and plugin
  * **Dependencies bring in external libraries needed to run or compile the project**
    * A dependency in Maven is a library (usually a .jar file) that the project requires to compile, test, or run. These dependencies are specified in the <dependencies> section of the pom.xml. 
    * Maven downloads the dependencies automatically from the specified repository and includes them in the project’s classpath. 
    * Example: If you need a logging library, you might add it as a dependency so it’s available during both compile-time and runtime.
  * **Plugins add functionality to perform specific tasks in the build lifecycle, such as compiling or testing.**
    * A plugin in Maven is a tool that executes specific tasks during the build process. Plugins handle various build phases, such as compiling code, running tests, packaging, etc. They are defined in the <build><plugins> section of the pom.xml. 
    * Maven plugins are executed at different stages of the Maven build lifecycle. For example, the maven-compiler-plugin is used to compile source code, while the maven-surefire-plugin is used to run tests. 
    * Example: If you want to compile your Java code with specific options, you would configure the maven-compiler-plugin.