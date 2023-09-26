# CI/CD with Jenkins

This is my Continuous Integration and Continuous Deployment.

I use various tools in one build pipeline, Maven as a automating tool to build my Java project, which is stored on Github and is accessed from the Jenkins build.
My build will ran Maven commands on the project to restart the project upon changes, then the project will be stored on Nexus Artifact Repository for versioning and storing.
The pipeline build is finally integrated with Apache Tomcat to run the project on the web.

The servers are run on AWS EC2 instances & the pipeline is written in the Groovy script (see "Jenkinsfile-cicd").

The running Build on Jenkins:


![Jenkinsbuild](https://github.com/Semir-Devops/CICD-Jenkins/assets/144611511/22f3b73c-1aab-4b85-9f34-ec778644dca7)


The project running on Tomcat: 

![tomcat(CICD)](https://github.com/Semir-Devops/CICD-Jenkins/assets/144611511/f95bd546-af2e-4fe6-aa77-5d9907fb14e4)

The Nexus Repository that stores my application:

![NexusRepo](https://github.com/Semir-Devops/CICD-Jenkins/assets/144611511/9da2a86f-30c6-453a-a846-cdaf3486978f)
