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
* After exercise 2, everyone should know what the principles of a decent pipeline are.

## Exercise

We should set a challenge here to build a multi stage pipeline for Restful Booker:

* Run a security scanner after build (I have some documentation on that in this folder now)
* Build the app and run the unit and integration tests on dev
* Deploy the app and run end to end tests on system test
* Deploy the app and run end to end tests with a smoke test tag on stage
* Add a paused for input sections to the pipeline
* Build jenkins jobs for all the above, then get them to build the pipeline