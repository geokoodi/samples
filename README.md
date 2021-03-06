# samples
Choco-solver in practice
========================


This project hosts samples based on [choco-solver-4.0.5](https://github.com/chocoteam/choco-solver/releases/tag/4.0.5).
This is mainly a source projet and no executable jar provided.
To easily play around with choco-solver, one needs:
- [Java Development Kit 8](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
- [Maven3](http://maven.apache.org/download.cgi) _(optional but recommended)_
- on IDE (eclipse, IntelliJ IDEA, etc)

Easy way (with maven)
---------------------

1. Download the [latest source code](https://github.com/chocoteam/samples/releases/latest) (zip or tar.gz).
2. Un-archive the file and go to samples directory.
3. Open a terminal and run the maven command:
    ```bash
    mvn clean install -DskipTests
    ```
4. Then open the samples project with your IDE.
Depending on your IDE, maven provides commands to configure your environment.
For example, `mvn idea:idea` will generate _*.ipr_ file.

To run a sample, select it `org.chocosolver.samples.*` subpackages and call the main method.
For example, select `org.chocosolver.samples.integer.Nonogram` 
and run the class with the following program arguments `-f -d rabbit`.


Alternative to step 3. (without maven)
--------------------------------------

Create a new project based on samples source and downloads required dependencies:
- [choco-solver-4.0.5](http://mvnrepository.com/artifact/org.choco-solver/choco-solver/4.0.5)
- [pf4cs-1.0.5](http://mvnrepository.com/artifact/org.choco-solver/pf4cs/1.0.5)
- [args4j-2.33](http://mvnrepository.com/artifact/args4j/args4j/2.33)

Add them to the classpath of the new project.
