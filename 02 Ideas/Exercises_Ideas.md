# Overview Planning

## Preparing the Attendees (30 mins)

### Introductory Presentation

* Signposting
* What we want to achieve
* What exercises we'll do to achieve those aims
* What is a pipeline in this context?

### Learn who's in the room

* Introduce yourselves to your table
* Scenario - Does your team have an automated deployment pipeline (hands up)? If you needed to investigate a problem with your teams deployment pipeline. How confident would you be?
  * 0
    * Most people in the room are 0-5 then we know we need to do some basics
  * 5
    * Most people are here, then we can skip ahead a bit
  * 10
  * Mix the confident and the less so together
  * Groups of 4 or 5 (work with people you don't know) - we should pick

### Setup

* Docker
* Pull a jenkins docker image and do the setup steps - prerequisite
* Git installed on the jenkins - some guidance on plugins
* Clone and install restful booker
* Github account

## Exercises

### Recognise the terminology and techniques applied to building and maintaining deployment pipelines (10-20mins)

* This is our 0-5 exercise

### Understand the principles of pipeline design through analysing new or existing tests, test strategies and environments available (20-30mins)

* Take a test strategy for restful booker - build a pipeline with various steps
* Paper exercise - values of the users, risks of the application

### Apply these principles to building a multi stage pipeline with Jenkins (The Rest)

* Basics of Jenkins - jobs, credentials, source control, branch of restful booker with a Jenkinsfile
* Build a dev version, then run acceptance test
* Intentionally break some tests, debug and fix
* Build something like UAT, then have a pause in your pipeline, exploratory testing
* Security scanner step
* If all good deploy to Prod
