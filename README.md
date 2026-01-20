# simple-java-maven-app

This repository is for the
[Build a Java app with Maven](https://jenkins.io/doc/tutorials/build-a-java-app-with-maven/)
tutorial in the [Jenkins User Documentation](https://jenkins.io/doc/).

The repository contains a simple Java application which outputs the string
"Hello world!" and is accompanied by a couple of unit tests to check that the
main application works as expected. The results of these tests are saved to a
JUnit XML report.

The `jenkins` directory contains an example of the `Jenkinsfile` (i.e. Pipeline)
you'll be creating yourself during the tutorial and the `jenkins/scripts` subdirectory
contains a shell script with commands that are executed when Jenkins processes
the "Deliver" stage of your Pipeline.

1) What is the CI/CD?
What is Jenkins?
Jenkins is one of the most widely used tools for automation in CI/CD pipelines.
 It is useful not only for developers, but also for operations and IT engineers who may not have a strong development background.
DevOps Context
•	In DevOps, operations engineers work closely with developers.
•	Developers create and modify application code.
•	Jenkins automates the process of building and testing this code.
Example Application
•	Example used: Java application.
•	Source code is the starting point.
•	Common build tools:
•	Maven
•	Gradle
•	Output example: a JAR file.

<img width="1445" height="652" alt="image" src="https://github.com/user-attachments/assets/d774f1fe-a31a-4255-a722-c18dfe12702d" />
