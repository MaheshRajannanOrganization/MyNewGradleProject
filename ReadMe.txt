

http://www.vogella.com/tutorials/EclipseGradle/article.html

http://www.journaldev.com/8118/java-simple-example-with-gradle-eclipse-plugin

gradlew...

it is a wrapper. it downloads necessary dependencies.

In maven you will write plugins.

just like pom.xml , with convention over configuration, except it is highly extendable
to the potential of java itself.

Gradle

Java

primarily building things…

setup ssh properly.

main branch alone is sufficient.


---command line.

export GRADLE_HOME=/Users/maheshrajannan/Installers/gradle-2.12
export PATH=$PATH:/Users/maheshrajannan/Installers/gradle-2.12/bin

--Init plugin.

http://www.mkyong.com/gradle/gradle-create-java-project-structure-automatically/

--

https://docs.gradle.org/current/userguide/plugins.html

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures

Closure is an object with the method, and the context in which the method was created.

*********Executing Custom Plugin********

maheshs-mbp-2:customPlugin maheshrajannan$ ls
build.gradle
maheshs-mbp-2:customPlugin maheshrajannan$ gradle tasks --all
:tasks

------------------------------------------------------------
All tasks runnable from root project
------------------------------------------------------------

Build Setup tasks
-----------------
init - Initializes a new Gradle build. [incubating]
wrapper - Generates Gradle wrapper files. [incubating]

Help tasks
----------
buildEnvironment - Displays all buildscript dependencies declared in root project 'customPlugin'.
components - Displays the components produced by root project 'customPlugin'. [incubating]
dependencies - Displays all dependencies declared in root project 'customPlugin'.
dependencyInsight - Displays the insight into a specific dependency in root project 'customPlugin'.
help - Displays a help message.
model - Displays the configuration model of root project 'customPlugin'. [incubating]
projects - Displays the sub-projects of root project 'customPlugin'.
properties - Displays the properties of root project 'customPlugin'.
tasks - Displays the tasks runnable from root project 'customPlugin'.

Other tasks
-----------
hello

BUILD SUCCESSFUL

Total time: 1.931 secs

This build could be faster, please consider using the Gradle Daemon: https://docs.gradle.org/2.12/userguide/gradle_daemon.html
maheshs-mbp-2:customPlugin maheshrajannan$ gradle -q hello
Hello from the GreetingPlugin
maheshs-mbp-2:customPlugin maheshrajannan$ pwd
/Users/maheshrajannan/Installers/gradle-2.12/samples/userguide/organizeBuildLogic/customPlugin
maheshs-mbp-2:customPlugin maheshrajannan$ 


Example 39.1. A custom plugin

build.gradle

*************************

http://igorpopov.io/2014/05/01/understanding-gradle/