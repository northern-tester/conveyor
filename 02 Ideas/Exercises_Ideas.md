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
* Clone and install restful booker - explain a bit about restful booker
* Github account

## Exercises

### Recognise the terminology and techniques applied to building and maintaining deployment pipelines (10-20mins)

* This is our 0-5 exercise
* Docker - introduction to containers
  * Get everyone installed
  * Difference between containers, VM and host
  * Match terminology to term
* Jenkins - introduction to pipelines
  * Get everyone installed, setup steps
  * How/what is a pipeline - codification of a set of manual steps
* Github - clone the repos needed

### Build a multi stage pipeline with Jenkins (The Rest)

* Snippets of code - steps in the declarative style
* Initial walkthrough to get a simple pipeline setup
* Basics of Jenkins - agents, jobs, credentials, source control, branch of restful booker with a Jenkinsfile
* Parallel vs Sequential steps - tests maybe able to run in parallel, security scans can take a little longer
* Build a dev version, then run acceptance test
* Intentionally break some tests, debug and fix - before workshop - get the attendees to fix them
* Build something like UAT, then have a pause in your pipeline, exploratory testing
* Security scanner step
* If all good deploy to Prod

### Understand the principles of pipeline design through analysing new or existing tests, test strategies and environments available (20-30mins)

* Pipelines not only automated, they can have manual steps
* They need to report on their progress, alert on failure
* Ask for examples of how their pipelines work - draw it.
* Timing is important - how long a build takes - introduce parallelism
* Take a test strategy for restful booker - build a pipeline with various steps
  * Pauses at test so testers can get builds when ready
* Agile testing quadrants - acceptance test, unit...
* Environments to step through - dev, int, test, pre-prod, prod.
* Paper exercise - values of the users, risks of the application


