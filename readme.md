# CI/CD with Jenkins

This is my Continuous Integration and Continuous Deployment.

I use various tools in one build pipeline, Maven as a automating tool to build my Java project, which is stored on Github and is accessed from the Jenkins build.
My build will ran Maven commands on the project to restart the project upon changes, then the project will be stored on Nexus Artifact Repository for versioning and storing.
The pipeline build is finally integrated with Apache Tomcat to run the project on the web.

The servers are run on AWS EC2 instances & the pipeline is written in the Groovy script.

The running Build on Jenkins:

