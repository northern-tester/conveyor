# Apply these principles to building a multi stage pipeline with Jenkins (The Rest)

* Snippets of code - steps in the declarative style
* Initial walkthrough to get a simple pipeline setup
* Basics of Jenkins - agents, jobs, credentials, source control, branch of restful booker with a Jenkinsfile
* Parallel vs Sequential steps - tests maybe able to run in parallel, security scans can take a little longer
* Build a dev version, then run acceptance test
* Intentionally break some tests, debug and fix - before workshop - get the attendees to fix them
* Build something like UAT, then have a pause in your pipeline, exploratory testing
* Security scanner step
* If all good deploy to Prod

## Starting Point

* After exercise 1, everyone should have a pipeline with the basics of stages, steps, agents and decisions.

## Exercise

We should set a challenge here to build a multi stage pipeline for Restful Booker:

* Run a security scanner after build (I have some documentation on that in this folder now)
* Build the app and run the unit and integration tests on dev
* Deploy the app and run end to end tests on system test
* Deploy the app and run end to end tests with a smoke test tag on stage
* Add a paused for input sections to the pipeline
* Build jenkins jobs for all the above, then get them to build the pipeline

* Step by Step
  * Set up Dev, Int and Deploy jobs
    * Dev - build the app, run unit tests
    * Int - run integration tests
    * Deploy - deploy artefacts
  * Introduce build from jobs to the pipeline
  * Pause in the exercise to talk about this pattern
    * Everything in the pipeline - pipeline as code, everything in one place
    * Running existing jobs in pipeline - can take advantage of existing jobs, which might be an easier starting point
  * Introduce manual steps with input methods (exploratory test, deploy)
  * Then add paralellisation - placeholders for Security Scan.
  * Optional challenge to get the ZAP scanner up and running.
  * This could be code cleanliness tooling like Sonarqube...
