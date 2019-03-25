# Understand the principles of pipeline design through analysing new or existing tests, test strategies and environments available (20-30mins)

* Pipelines not only automated, they can have manual steps
* They need to report on their progress, alert on failure
* Ask for examples of how their pipelines work - draw it.
* Timing is important - how long a build takes - introduce parallelism
* Take a test strategy for restful booker - build a pipeline with various steps
  * Pauses at test so testers can get builds when ready
* Agile testing quadrants - acceptance test, unit...
* Environments to step through - dev, int, test, pre-prod, prod.
* Paper exercise - values of the users, risks of the application
* Exercise 1 - Jenkins running and a simple pipeline with agents, steps. stages, decisions

## Exercise details

* We want to be able to teach the principles of pipeline design, which begs the question, what are the principles of pipeline design?
  * You already have something of a pipeline, just not codified yet.
  * Steps can be manual and automated, with a preference to automation over time.
  * Complexity in your pipeline is heuristic for complexity in your application and its environments. Where possible don't codify it.
  * Build things once, don't rebuild artifacts for each stage of your pipeline.
  * Production like is desired, but can be by degrees. If you have a thousand webservers that might not be replicable in test, but you can cluster with the same components.
  * Fast concise feedback mechanism - needs to be timely.
  * Needs to be testable - it is code and makes decisions based on inputs. How can we make it testable.
  * Resilient - put you back into a known state.
  * Increasing confidence throughout the pipeline.
  * Excellent configuartion management.
  * Make your pipeline wide, not long - use paralellism
  * Can we use CALMS as a summary here, then fit the principles in.
  * Introduce CALMS as a model then fit the principles of pipelines in. Create a handout.

* In terms of types of exercise, we want to introduce some realism in there.
* Want to try and avoid lots of looking at paper and reading to convey a scenario. Best to try and get them to discuss.
* Question is shall do an unrealistic restful booker thing or get them to pipeline workshop their own pipelines.
* What about the testing of their own pipelines?
  * Pipeline using value stream mapping - with different types of testing in there.
  * Scenario that everyone can do:
    * A number of environments and how they compare to live
    * A description of the system itself - microservices that are on containers that autoscale - show this as a dataflow
    * Types of testing strategy - use the agile testing quadrants
    * Groups of 4 - get them to pick a pipeline owner and ask them to describe the three aspects above for their own systems.
    * Ask what they are comfortable sharing.
    * Use value stream mapping as a concept 
    * Provide a key for what each stage should look like.
