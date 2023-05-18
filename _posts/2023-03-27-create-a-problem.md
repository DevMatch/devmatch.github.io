---
layout: post
title: "Creating a problem"
date:   2019-01-20 23:45:29 -0800
categories: docs
---

# DevMatch engineering challenges

The DevMatch platform helps you to host short (1-hour) engineering challenges. These challenges are meant to be representative of day to day activities of a software engineer. There are [plenty of examples](https://www.trytapioca.com/library-of-assessments) of these challenges out there that you can borrow inspiration from. 

DevMatch grabs concepts from competitive programming. You provide a statement to the participant and sometimes a starting point, like a pre-existing code repository. Then, the user changes the code or creates code from scratch that is submitted to DevMatch. DevMatch then runs the **evaluator**, which scores the solution based on pre-defined **test cases**. The test cases are returned to the user as a submission score.

<!--
::: mermaid
sequenceDiagram
    autonumber
    actor User
    participant DevMatch
    participant Challenge
    User->>DevMatch: Open Problem
    DevMatch->>Challenge: Open Problem
    Note right of Challenge: prerequisites()
    Note right of Challenge: openProblem()
    Note right of Challenge: getProblemStatement()
    Challenge->>DevMatch: Statement
    DevMatch->>User: Statement
    loop SolveProblem
        User->>DevMatch: Submit
        DevMatch->>Challenge: Submit
        Note right of Challenge: getTestCase()
        Note right of Challenge: validate()
        Challenge->>DevMatch: Test cases
        DevMatch->>User: Test cases
    end
:::
-->

# Quick start

1. Clone or download this repo: `git@github.com:DevMatch/DevMatch-SDK.git`
2. Open `validator\src\validator.ts`
3. Install dependencies `npm i`
4. Install dependencies `npm run publish`
5. Create a new problem in DevMatch and insert into the code section


# Creating a challenge


You need to define the following:

* An introduction that is 255 characters long.
* A statement.
* A time limit, less than 1 hour.
* A validator.

## Prepare
* Get the job description if you have it
* Get external source code and make sure you can run it
* Search online for sample take homes
* Define skills to assess
* Define the test cases

## Design the technical implications
  * Consider the verification mechanism. Unit tests? UI tests? Which framework?
  * Remove the boilerplate
  * Remove the external dependencies

##  Implement the verification
  * Insert testing framework
  * Write test cases
  * Write the CI pipeline if running in CI/CD build. This also includes publishing artifacts.
  * Write the DevMatch validator
  * put in source code version control

## Integrate with DevMatch
  * Make the UTs output a json that DevMatch can read

# Example

In this example we will create a challenge that asks a user to create a CLI tool. This tool will take two integers as arguments and print the sum of the two arguments. It should handle bad input such as non integers or the number of arguments.

* Prepare
  * There is no specific job description for this challenge.
  * We don't want to give the user any starting boilerplate code.
  * Pending.
  * The skills that we want to assess with this challange are: command line tools, nodejs, basic input output.
  * Some test cases include adding two integers, negative numbers, zero arguments, one argument, three arguments.
* Design
  * I will find a testing framework for CLIs
* Implementation.

I will start by creating an empty directory and git repo where I can put my validator:

```
mkdir cli-sum
git init
```

Then, I need to create 3 folders, `problem`, `validator`:

```
mkdir problem validator docs
```

* `problem` contains the root of the repo that the user will see.
* `validator` is where you write the code that validates the problem is correct.

We don't want to give the user any starting point code, but we might want to add a readme.txt to problem for them to see. Let's start writing the validor.

## Validator

The validator needs to be written in JavaScript that runs on node.js. 


## Other considerations

* Installation of dependencies require resources out of the package managers main database?
* For example, installing `dynamodb-local` requires a download from AWS servers, the binary is not in NPM 

## Considerations on using CI
DevMatch can use traditional CI/CD builds to run validators. DevMatch will need to:

* Trigger a build. This means that the definition (usually Yaml) has already been created.
* Add metadata to the build instance; this will be the DevMatch build id.
* Continuously query the state of a given build by ID.
* Fetch artifacts from a finished build.

