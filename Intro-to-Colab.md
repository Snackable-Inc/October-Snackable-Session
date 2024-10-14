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

But that's still not _quite_ clear enough. So let's cut back on the technical mumbo-jumbo and get to the heart of what GitHub is...

## Let's define GitHub by the problem it solves:

When you have just a small number of people working on a project - let's say two or three people - collaboration, communication, and managing code is easy. You can just use email, chat, and share files and versions as you please. But as the number of people working on a project grows and the lines of code increases, the complexity of managing the project grows as well. This is where GitHub comes in.

Some typical challenges that arise are: multiple people making different contributions, tracking bugs, taking care of security vulnerabilities, planning changes and improvements and delivering new features, and just the day-to-day of managing your codebase.

The problem GitHub solves is this spiralling chaos that arises from a project as it grows in size and complexity, and the added workload you have when managing more and more people as your team grows too.

In the simplest terms, GitHub is a platform where you can store your code, manage your development projects, and collaborate with your teammates, and - as managers - keep track of what your team is doing.

We're going to scrap the powerpoints for today, and instead just get hands on to show some of the basics of how you can do all this. Let's start off with some of the fundemental parts of GitHub.

## The Core Elements of Collaboration on GitHub

### Repositories

Think of repositories as a storage space for your project. It will contain all the files and folders that make up your project, and it will also track the changes that are made to those files and folders over time - this is the "commit history", and this is what is the main part of what we're referring to when we talk about "version control" on GitHub.

To facilitate collaboration with multiple people, repositories also have branches. A branch is a parallel version of the repository that you can work on without impacting what your teammates are working on. These are used when you want to work on a new feature, fix a bug, or experiment with a new idea, for example. When you're ready to merge your changes into the main branch, you can create a pull request. We'll dive into that now...

### Branching vs Forking

Branching and forking are two ways to create a copy of a repository.

Let me focus on one thing first: the `main` branch. This is the default branch for a repository. This is usually the branch from which the repository is cloned, and the branch from which deployments of an application are built.

When you create a new branch, you are creating a copy of the repository that is still connected to the original repository under the same account. You can make changes to the branch, and then create a pull request to merge your changes back into the `main` branch.

When you create a fork, you are creating a copy of the repository that is _not_ connected to the original repository. Forking requires creating a copy of the code in a new repository, and optionally under a different account. You can still merge your changes back into the original repository from your fork via a pull request later on if you need to.

> [!NOTE]
> It can often also require more work to keep the fork up to date with the original repository.

To recap: the difference between the two is that a branch is a copy of the repository that is still connected to the original repository, while a fork is a copy of the repository that is _not_ connected to the original repository. Instead, a fork of the repository will typically exist in your own account, and you can work on it without affecting - or being affected by - the original repository.

They're used in different situations. A good example of when you'd use a branch is when you're working on a new feature or bug fix within an existing project. You can create a branch, make your changes, and then create a pull request to merge your changes back into the `main` branch.

Branching is typically the simplest way to create a copy of a repository to work on your contributions - everything stays within the same repository and within the same account.

A good example of when you'd use a fork is when you want to make a copy of a repository that you don't have direct write access to. You can fork the repository, make your changes, and then create a pull request to merge your changes back into the original repository.

Another situation of when you'd like to use a fork is to create a new version of an existing project - maybe you want to use an existing project as a template that you want to build on or localise, or you simply don't like the direction that the original project is going and want to go your own way.

### Pull Requests

So you've brached or forked the repository and you've made your changes. You'll now want to merge it into the main branch. This is where pull requests come in.

Pull requests are a way to propose your changes and have them reviewed and tested by your team before they are merged into the `main` branch. They are a way to discuss your changes, get feedback, make further changes if needed, and ensure that your changes are in line with the project's goals and standards.

### Issues

Software projects will always need changes, updates, and bug-fixes. These are typically initiated in Issues.

Issues are a simple way to start a bit of documentation linked to the code in a repository about a problem, a feature request, or simply a question that may lead to a larger piece of work. Within the issue, you can discuss the problem, assign it as a task to someone, and track the progress of the work, and do that all with formatted text, images, videos, links, specific lines of code, and other issues or pull requests.

You can create a branch to work on the bug/update/ides described right from within in the issue.

> [!TIP]
> Issues can be organised with [GitHub projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) too. This enables you to organise them into a Kanban board, Gantt chart, or a table organised by priority. You can assign them to team members, set deadlines, and track the progress of the Issues and PRs within the project board view.

In short, Issues are not just for bugs! They can be used for anything that needs to be tracked, such as feature requests, questions, or even just general discussion.

## Types of Account

There are three types of account on GitHub: User, Organization, and Enterprise. They follow a hierarchy, with an Enterprise account being the "parent" account that can manage multiple organizations, and organizations being the account that can manage multiple users and repositories.

### What is an Organization?

Work on GitHub (i.e. repositories, issues, pull requests, etc.) are done within an organization, which will be the owner of the work. Organizations can be public or private, and can have multiple teams and repositories.

They are maintained by owners and administrators, who can manage the organization's settings, billing, and membership.

### What is an Enterprise?

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

### Enterprise Managed Users (EMUs)

Enterprise Managed Users are a special typr of user account that are managed by an Enterprise - they belong to the Enterprise, rather than the individual. This means that the Enterprise can enforce certain policies on the user, such as access and authentication, SSO, 2FA, and Enterprise administrators can also see the user's activity across all the organisations in the Enterprise.

## On top of that...

That's the essential stuff that makes GitHub a valuable tool for collaborating with others on software projects. There's a lot more to it though!

On top of all that, you can build your own custom automations to all of these features - you can use GitHub Apps, Actions, and the GitHub API to automate tasks such as:

* Code reviews
* Continuous integration and delivery
* Code quality checks
* Testing and status checks
* Auto-assignment of issues and code reviews
* Labeling and triaging issues
* Enforcing branch protection rules

[Read more here.](./Extras.md)