# DEPLOY01_HELLO_WORLD

#See Deployment#1.pdf for instructions


<h1>Purpose</h1>

The purpose of this deployment was to get hands on experience with utilizing AWS, specifically EC2 and setting up a software called Jenkins to build standard pipeline that would access this git repository and build out the application that is in the folder.

<h2>Jenkins</h2>

Jenkins is a software written in Java that runs on a computer and the use-case for Jenkins in this deployment is to set up a Jenkins project that would pull from this repository, read the Jenkinsfile, which holds the instructions for building this application, and then capturing a screenshot of the completion.

Outside of this project, Jenkins can be used for multiple projects and building cases including building python applications, testing the application, deploying onto another connected service and it can all be done either through a webhook update alert to Jenkins when a new repository update is sent to Jenkins or on a timed schedule.

<h2>Why this is important</h2>

By setting a server that can automate the build process, be notified when changes are made and act on them in a repository as opposed to having things done in a manual fashion, it reduces down time for developers and any real world testing that may need to be done in a timely fashion. The benefits of this in the long run and on a large enough team could be several hours to days or perhaps even weeks of time saved in deployment times when done appropriately and to scale.
