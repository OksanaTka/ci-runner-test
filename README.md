# CI Runner Test

This repository is a simple test project for experimenting with **GitHub Actions self-hosted runners**.

## Purpose 

The goal of this repository is to learn how to:

• Register a self-hosted runner
• Connect a local machine to GitHub Actions
• Run workflows on a personal machine instead of GitHub-hosted runners

## Setup

A self-hosted runner was installed locally and connected to this repository.

When a workflow runs, GitHub sends the job to the local runner, which executes the steps on the machine.

## Example Workflow

The test workflow prints basic system information from the runner machine, such as:

* hostname
* current user
* working directory
* operating system details

This confirms that the workflow is executed on the **local machine**.

## Technologies

* GitHub Actions
* Self-Hosted Runner
* macOS (ARM64)

## How to run

1. Start the self-hosted runner on your machine:

```
cd actions-runner
./run.sh
```

2. Go to the repository in GitHub.

3. Open the **Actions** tab.

4. Select the workflow **Test self hosted runner**.

5. Click **Run workflow**.

GitHub will send the job to the self-hosted runner, and it will execute the workflow on the local machine.
