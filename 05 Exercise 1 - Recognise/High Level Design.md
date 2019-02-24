# Recognise the terminology and techniques applied to building and maintaining deployment pipelines (10-20mins)

* This is our 0-5 exercise
* Docker - introduction to containers
  * Get everyone installed
  * Difference between containers, VM and host
* Jenkins - introduction to pipelines
  * Get everyone installed, setup steps
  * How/what is a pipeline - codification of a set of manual steps
* Github - clone the repos needed

## Building a working pipeline by getting installed

### Experience - Do Something

* Docker
  * Get everyone to check their installs by running a number of commands
* Jenkins
  * Do the pull latest jenkins instance and maybe a docker agent (prompt to do this before in the pre-reqs)
  * Also, do the jenkins login thing where we cat the code and create a user
  * Create a job that is a pipeline with a jenkinsfile, more of a sandbox.
  * Add a parameter to the job
  * Introduce concepts within - code along style.
    * Agents
    * Stages
    * Steps
    * Decisions (when) - based on the parameter

### Reflect - Review the experience

* Show of hands for installs
* Ask the audience - what is an agent, stage, step, expression

### Learn - Conclude from the reflection

* How many stages might your current testing pipeline have?
* Why might you use different agents in your pipeline?

### Experiment - Try out what you have learnt

* Build a pipeline with 3 stages - dev, integration, stage.
* Echo out some statement.