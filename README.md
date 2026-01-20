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

Why This Matters
In the past, developers on a team might work in isolation for an extended period of time and only merge their changes to the master branch once their work was completed. This made merging code changes difficult and time-consuming, and also resulted in bugs accumulating for a long time without correction. These factors made it harder to deliver updates to customers quickly.
•	The whole process is automated.
•	Developers only need to commit code.
•	Jenkins handles:
•	Detecting changes
•	Building the application
•	Running tests
Continuous Integration Concept
•	Every code change is built and tested automatically.
•	If a test fails:
•	The developer is immediately informed.
•	The developer must fix the issue and commit again.
•	This ensures the codebase is always in a working state.
What is the Continuous Delivery?
CD is the stage after CI. Once the application is built and tested successfully, CD is responsible for deploying the application.
CI -> Build - Test
CD -> Package - Push - Deploy

<img width="1198" height="369" alt="image" src="https://github.com/user-attachments/assets/6dbaa88c-7fd1-4359-a5a9-dc97c5fb2d27" />

Example CD Flow with Jenkins
After tests pass:
1.	Build Docker image from the application.
2.	Push the image to a container repository.
3.	Update Kubernetes deployment file with the new image.
4.	Deploy the application to Kubernetes.
All these steps are added as pipeline stages in Jenkins.
 
Jenkins can be configured so that:
•	If tests pass, it automatically:
•	Builds the Docker image
•	Pushes it to the repository
•	Deploys it to the environment
This removes manual work:)
 
Note:  Jenkins can also be used for
•	Scheduled clean-up jobs
•	Automated releases
•	Standalone build jobs
Continuous Integration vs Continuous Delivery
With continuous delivery, every code change is built, tested, and then pushed to a non-production testing or staging environment. There can be multiple, parallel test stages before a production deployment. The difference between continuous delivery and continuous deployment is the presence of a manual approval to update to production. With continuous deployment, production happens automatically without explicit approval. 
Continuous delivery automates the entire software release process. Every revision that is committed triggers an automated flow that builds, tests, and then stages the update. The final decision to deploy to a live production environment is triggered by the developer.



