# CI/CD platform save you time and guard your application deployment.

A CI/CD (Continuous Integration and Continuous Deployment) platform can automate the development, testing, and deployment for software developers.

## CI/CD is there to take over repetative tasks

Using such a platform will save you time as a developer by automating repetitive operations. Testing code changes and making, distribute those changes to different environments, performing scheduled tests and even auto-correct your syntax preference.
Any one of those pipelines, and more, will run automagically whenever new code is uploaded to a source code repository. This enables you to detect and resolve difficulties early in the development process before they become more complex and time-consuming. Automating the deployment process allows you to distribute code changes to several environments with a single click.

## Example of a CI/CD pipeline

The developer is still responsible for authoring and testing the code in this example, but the CI/CD pipeline automates the chores of building, deploying, and testing the code changes. This can save the developer time by removing the requirement to build and test scripts manually and automating the deployment process.

1. Changes to the code are published to a source code repository (e.g. GitHub).
1. CI/CD pipeline initiates an automated build process in which the code is built and packaged.
1. Automated tests are run on the freshly created code to detect any problems or flaws.
1. If the tests are successful, the code is deployed to a staging environment for additional testing.
1. The code can be deployed to the production environment only once it has passed all tests.

Furthermore, by automating the testing process, the CI/CD pipeline guarantees that code is completely tested before being released to the production environment. This can assist to lessen the likelihood of problems or defects in the production environment while also making the development process more efficient.

## Does my project need CI/CD?

A few use cases where you can benefit from incorporating a CI/CD pipeline into your project:

1. Decrease the chance of mistakes by allowing CI/CD to perform repetitive operations such as creating, testing, and deploying code.
1. Resolve issues early in the development process, by setting up continuous integration testing, before they become harder to resolve.
1. Deliver code updates faster by automating the deployment process, and delivering code updates to different environments.
1. Enhance code quality by allowing a CI/CD pipeline to ensure the code adheres to your coding standards.

That being said, it's crucial to remember that putting up a CI/CD pipeline takes time and work, that's where you can make use of [agnostic CI/CD scripts](./agnostic-scripts.md), that can reduce the set up time significantly. Overall, it's worthwhile to examine if a CI/CD pipeline might be useful for your project, and to compare the possible advantages against the time and work necessary to put it up.
