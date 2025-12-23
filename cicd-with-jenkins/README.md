# Intro to Jenkins & CICD

## What is CI? Benefits?

* Continuous Integration
* automatically merging code
* Triggered by: Developers frequently pushing the code changes to shared repo
* Tests are run automatically on the code before it is integrated into the main code
  
Benefits
* Help you to identify and resolve bugs early
  * Reduces costs
* Helps to maintain a stable and functional software build 

## What is CD? Benefits?

* Can mean:
  * Continuous Delivery (manual sign off/approval), OR
  * Continuous Deployment (automatically deploys code to production)

Continuous Delivery (manual sign off/approval)
* ensure software is always in a deployable state, ready/can be pushed to production any time
* often involves producing deployable artifact
* requires a manual release decision
* benefit:
  * always have a deployable artifact ready to deploy to end users

Continuous Deployment (automatically deploys code to production)
* extends Continuous Delivery by automating the final step of deploying to production
* no manual intervention required
* benefit which is also a disadvantage:
  * removes the human approval, relies entirely on automated processes

## What is Jenkins?

* automation server
* open-source
* primarily used for CICD, but can automate much more

## Why use Jenkins? Benefits of using Jenkins? Disadvantages?

* Benefits:
  * Automation
  * Extensibility: Jenkins has over 1800 plugins
  * Scalability:  Jenkins server can scale easily by adding/using worker nodes/agents to run jobs
  * Community support
  * Cross-platform: Works across Windows, Linux, MacOS
  
* Disadvantages:
  * Can be complex for beginners
  * Maintenance overhead
  * Resource-intensive when running multiple jobs
  * User interface: outdated?

## Stages of Jenkins

A typical Jenkins CICD pipeline involves the following stages:
1. Source Code Management(SCM)
2. Build: Compile the code, build into executable artifact
3. Test: Automated tests (unit, integration, etc)
4. Package: Package into deployable artifact
5. (If using Cont. Deployment) The package is deployed into the target environment e. g. test, production
6. (If using Cont. Deployment) Monitor: Monitoring tools may be deployed/configured to observe performance, log issues, etc after deployment

## What alternatives are there for Jenkins

* GitLab CI
* GitHub Actions
* CircleCI
* Travis CI
* Bamboo
* TeamCity
* GoCD
* Azure DevOps (Azure Pipelines to run the CICD pipelines)

## Why build a pipeline? Business value?

* cost savings - automating repetitive processes
* faster time to market
* reduced risk
* improved quality through continuous feedback and improvement