# Contributing Guidelines

👍🎉 First off, thanks for taking the time to contribute! 🎉👍

The following is a set of guidelines for contributing to **Privacy evaluator for Machine Learning models**, which is an open-source project hosted on GitHub. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

You can also find [README](https://github.com/privML/privacy-evaluator) and [CODE OF CONDUCT](https://github.com/privML/privacy-evaluator).

# How Can I Contribute

## Issues
In order to achieve an efficient workflow, there should be an easily accessible resource to get information on the current state of development. We use [Projects table](https://github.com/orgs/privML/projects/1) for that. That way, a developer can quickly select an open issue that is ready for implementation and stakeholders can get an overview of the progress. Each time you want to solve a new problem, create an Issue, give a short description of the problem, its acceptance criteria, assign people, tag if needed.

## Branches

### Special branches

- `main`: the current state of development

### Regular branches

Branches that are being worked on should be named according to the following schema:  
`[TYPE]/[ISSUENUMBER]-[SHORT-SLUG]`, e.g. `feat/22-membership-inference-attack`  

## Commits

Regular commit messages should adhere to the following format:  
`[COMMIT MESSAGE]. #[ISSUE]`, e.g. `Improve contribution guidelines. #44`

`[COMMIT MESSAGE]` should be formulated, such that this statement makes sense:

> When applied, this commit will `[COMMIT MESSAGE]`.

Note: "When applied, this commit will" is just a _grammatical guideline_. It does **not** belong into the message.

## Pull requests

Pull requests are used to validate the functionality and code for an issue.
Before a piece of code can make it to `main`, it has to undergo a pull request.

### Creating

When creating a pull request, refer to the relevant issues in the description.
Describe broadly how the issue was implemented.

For the title of the PR, use the short description you would use for the [merge commit](#merging) (without the type and scope).

### Reviewing

**Please review pull requests assigned to you.**  
Take some time to look at pull requests.
Other people want to get their features done as well.
This way we help each other, and keep the proccess moving.
When reviewing, apply common sense.

### Merging

When merging a PR, use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0-beta.4/) for the commit message, with some additions:

> {TYPE}([SCOPE]): [DESCRIPTION]
>
> [DETAILS]
>
> See ![MERGE REQUEST NUMBER].  
> Closes #[ISSUE NUMBER].

`{TYPE}` should be one of (select the first that applies):

- `feat`: A new feature will be introduced
- `fix`: A defect/bug/etc. will be fixed
- `test`: More tests will be added
- `docs`: Documentation will be added/updated
- `refactor`: Internals will be reworked
- `perf`: Performance will be improved
- `style`: Code style will be applied/changed
- `chore`: Generic catch all

The `([SCOPE])` is optional, but try to specify it (e.g. `inference-attack`, `inversion-attack`).  
Use the [`BREAKING CHANGE:` notation](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#commit-message-with-optional-to-draw-attention-to-breaking-change) if necessary, including the `!`.


## Code Style

Please always run `black` before submitting a pull request. You can install
`black` with `pip install black`.
