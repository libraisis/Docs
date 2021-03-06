# How To Contribute & Earn XUC

Yay! Kudos for being a part of Exchange Union & for helping to build the Exchange Union Daemon, our node software! Any contributions are welcome no matter how big or small. From typos and bug fixes to entire modules - you will be awarded with our token, XUC.

## Earning Rewards

Here's how it works:
1. Grab a task from [here](https://github.com/ExchangeUnion/xud/issues).
2. Each task carries a range of XUC to be earned, e.g. 50-100 XUC. The more complex the task, the higher the reward - grab a task which best fits your available time & skill set.
3. Leave a comment to let everyone know you'll be working on the task, and fork the repository to get started.
4. [Get in touch](https://gitter.im/exchangeunion/Lobby) for help along the way, especially for testing. Unfortunately our automation is still a work in progress! :/
5. When you feel ready, submit a pull request  against the `master` branch with your **ether address (!)** in the comment section.
6. For non-trivial changes, expect several rounds of review and testing to take place before your changes get merged into the master branch.
7. After a successful merge into the master branch we'll send the XUC reward to the ether address you provided in the comment section. For now this is all manual work on our end, but we would love for someone to propose a solution to automate this process (& propose a price tag)!

It goes without saying that you can exchange XUC to other assets on [various exchanges](https://www.exchangeunion.com/xuc).

If you see something missing or want to develop another cool feature or bug fix which doesn't have an issue yet, open one and we'll review and give it a price tag asap! We don't recommend working on things without an issue on github.

## Contribution Guidelines

If you are new to contributing to open sources projects on GitHub, check out [this how-to](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github/).

### Feature Branches & Pull Requests

We use [feature branches](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow) for devlopment. Each branch and pull request should focus on a particular feature or issue. Ensure that new branches are created from the latest code in `master`. A branch must be in a working and stable state before it can be merged into `master`.

Pull requests will be reviewed and changes may be requested. If changes are required, make new commits directly to the feature branch. If there have been conflicting commits to `master` since a feature branch was created, rebase the branch onto master using `git rebase`.

For pull requests of small scope, you may squash multiple commits into a single commit or a maintainer will squash them before merging. For more complex pull requests that touch many parts of the code or which contain commits from multiple contributors, please collapse commits by author and affected files or components of the project. This can be performed through an interactive rebase with `git rebase -i`. Use `git commit --amend` when fixing minor typos or bugs with the most recent commit. These practices help maintain a clean and coherent commit history while preserving contribution authorship.

### Linting & Testing

New test cases are appreciated for any pull requests that changes or adds new functionality. Although the current test suites are in early stages, thorough testing and code coverage is an important long term goal.

All code is linted with [tslint](https://github.com/palantir/tslint) using a slightly modified [tslint adaptation](https://github.com/progre/tslint-config-airbnb) of [Airbnb's javascript style guide](https://github.com/airbnb/javascript). Ensure that your contributions pass all linting rules by running `npm run lint` or using a code editor with a tslint plugin. Per-line or per-file exceptions to linting rules are allowable in certain cases.

### Commenting & Documentation

Make your code legible by using descriptive variable, function, and class names. For blocks of codes whose function is not readily apparent, add comments explaining what they do. If a pull request changes the interface to `xud` or introduces new functionality, update the README to describe these changes.

Xud uses [TypeDoc](http://typedoc.org/guides/doccomments/) and any comments documenting specific classes, methods, properties should follow this convention.

Commit messages should be concise and descriptive. For larger or more complex commits, add details of what has changed in the commit description.
