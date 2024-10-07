# Intro to GitHub Collaboration

## What is GitHub?

One of the trickiest questions to answer is just "What is GitHub?"

Not because there's no clear answer - but because there are different ways to answer it, and it can change depending on who's asking. Depending on where you look, you'll see different answers:

According to the infamous [rubber duck video](https://www.youtube.com/watch?v=pBy1zgt0XPc&ab_channel=GitHub):

> “It’s the largest, most complete development platform in the world!”

According to Wikipedia:

> "GitHub is a developer platform that allows developers to create, store, manage and share their code. It uses Git software, providing the distributed version control of access control, bug tracking, software feature requests, task management, continuous integration, and wikis for every project.”

[A little better](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git)…

> "GitHub is a cloud-based platform where you can store, share, and work together with others to write code.”

But it's all pretty vague, right? So let's cut back on the technical mumbo-jumbo and get to the heart of what GitHub is...

## Let's define GitHub by the problem it solves:

When you have just a small number of people working on a project - let's say two or three people - collaboration, communication, and managing code is easy. You can just use email, chat, and share files and versions as you please. But as the number of people working on a project grows, the complexity of managing the project grows as well. This is where GitHub comes in.

Some typical problems that arise will come from: multiple people making different contributions, tracking bugs, taking case of security vulnerabilities, planning changes and improvements, planning and delivering new features, and just the day-to-day aspects of managing your codebase.

The problem GitHub solves is this spiralling chaos that arises from a project as it grows in size and complexity, and the added workload you have when managing more and more people as your team grows too.

In the simplest terms, GitHub is a platform where you can store your code, manage your development projects, and collaborate with yout teammates, and - as managers - keep track of what your team is doing.

We're going to scrap the powerpoints for today, and instead just get hands on to show some of the basics of how you can do all this. Let's start of 

### Repositories

### Organisations

### Enterprises

#### What is an Enterprise?

An Enterprise is effectively a "parent" account that enables centralized management for multiple organizations.

Enterprise accounts are used to centrally manage policy and billing. Unlike organizations, enterprise accounts _cannot directly own resources_ like repositories, packages, or projects. Instead, these resources are owned by organizations within the enterprise account.

* Manage enterprise membership
* Manage billing and usage
* Configure security (such as SSO, IP allow lists, SSH, and 2FA)
* Stream audit and Git events data
* Use internal repositories
* Access features like GitHub Copilot Enterprise and Advanced Security
* Enforce policies for business rules or regulatory compliance

Enterprise accounts on GitHub come in two forms: GHES and GHEC.

#### Enterprise Managed Users (EMUs)

Enterprise Managed Users are user accounts that are managed by an Enterprise - they belong to the Enterprise, rather than the individual. This means that the Enterprise can enforce certain policies on the user, such as access and authentication, SSO, 2FA, and Enterprise administrators can also see the user's activity across all the organisations in the Enterprise.

### Branching

### Issues

### Pull Requests

## On top of that...

On top of all that, you can build your own custom automations to all of these features - you can use GitHub Apps, Actions, and the GitHub API to automate tasks such as:

* Code reviews
* Continuous integration and delivery
* Code quality checks
* Testing and status checks
* Auto-assignment of issues and code reviews
* Labeling and triaging issues
* Enforcing branch protection rules