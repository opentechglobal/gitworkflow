### Branch Naming

Branches created should be named using the following format:

```
{story type}-{2-3 word summary}-{pivotal tracker id}
```

`story-type` - Indicates the context of the branch and should be one of:

- ft == Feature
- bg == Bug
- ch == Chore
- rf == Refactor

`story-summary` - Short 2-3 words summary about what the branch contains

**Example**

```
ch-progressive-web-app-171145778
```

### PR Naming

The PR title should be named using the following format:

```
#[STORY_ID] Story description
```

**Example**

```
#171204615 Redirect to login page after password reset
```

### PR Description Template (Markdown)

The description of the PR should contain the following headings and corresponding content in Markdown format.

```md
#### What does this PR do?
#### Description of Task to be completed?
#### How should this be manually tested?
#### Any background context you want to provide?
#### Relevant pivotal tracker story(ies)?
#### Screenshots (if appropriate)
```

### Commits

Use atomic commits

An atomic commit is focused on one context and one context only.
By context we mean a single topic: a feature, bug fix, refactor, upgrade, task...

Atomic commits should be made with the format:

```
<type>(<scope>): <subject>``<BLANK LINE> <body> <BLANK LINE> <footer>

```

Any line cannot be longer than 100 characters, meaning be concise.

```<type>``` should be:

 * feature
 * bug
 * chore
 * release
 * refactor
 * documentation
 * style
 * test

```<scope>``` should be something specific to the commit change. For example:

 * login-page
 * dashboard
 * inactive-customers
 * logo and so on.

```<subject>``` text should:

 * use present tense eg: "add" not "added" or "adding"
 * not capitalize first letter i.e no "Add style to header"
 * not end with a dot (.)

**Message body (optional)** If a body is to be written, it should:

 * written in present tense.
 * include the reason for change and difference in the previous behaviour

**Message Footer** This should be used for referencing the issues using the following keywords: Start, Delivers, Fixes and Finishes. it should be inside a square bracket. Example:

```
[Start #171145778]
```

or in a case of multiple issues:

```
[Finishes #5438233, #5891837, #4988398]
```

## Example

chore(progressive-web-app):register service worker  
[Start #171145778]
