# Lesson 8 – CI/CD: Answers

## 1. What is the difference between CI and CD?
CI is the automatic process of testing and building code changes.
CD continues the process by preparing or automatically deploying the application.

## 2. What is the difference between a job and a step?
A step is a single command or action.
A job is a group of steps that run on the same runner.

## 3. What is the difference between uses and run?
run executes a shell command.
uses runs a reusable GitHub Action.

## 4. Why use a commit tag instead of latest?
A commit tag identifies an exact version of the code.
latest can change, making it harder to know which version is running.

## 5. How do we store a password needed by a pipeline?
We store it in GitHub Secrets, not directly in the workflow file.
The workflow accesses it using secrets.NAME.

## 6. What is GITHUB_TOKEN and why do we need permissions?
GITHUB_TOKEN is a temporary token created by GitHub for each workflow run.
permissions defines what the token is allowed to do.

## 7. What is a matrix?
A matrix runs the same job multiple times with different values.
In this project, it builds three services: backend, stats, and frontend.

## 8. What do you do when the pipeline fails?
I open the failed workflow, identify the failed job and step, read the logs, fix the problem, push the changes, and verify that the pipeline passes.