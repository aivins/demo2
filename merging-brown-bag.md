# Super quick overview

Version control with git. Git is distributed. Every person gets a full copy of the repository. Compare to other systems such as CVS, SVN, Perforce. There are others, such as Mercurial, but git seems to have won. Git has an acyclic dependency graph so every commit is guaranteed a linear history with no loops or circular references. Git is the version control software written by Linus Torvalds. Github, Gitlab, Bitbucket, etc, are web based services that support git and augment a repository with pull requests, issue tracking, collaboration, etc.

# Top level points

- Working copy, bunch of files under a folder
- Local commits
- Branches - just moving labels pointing towards a commit
- Merging and merge conflicts
- Rebasing?
- Pushing and pulling
- Pull Requests
- Tagging

# Working copy

Demonstrate this with a simple folder of files without any version control.
Show file structure in an editor.
Turn it into a git repo with "git init".

# Local commits

Demonstrate changes live in an editor.
Demonstrate a trivial string of commits.
Show the git log.
Show a diff between commits.

# Branches

Note how the main branch is just a pointer to the latest commit.
Create another branch and make a commit to it.
Switch between branches.
Show a diff between branches.

# Merging

Demonstrate a merge between the two branches
A merge commit - the commit that ties the two parents together.
Cause a deliberate merge conflict and resolve it.

# Rebasing

In git parlance it means replaying a set of commits on top of a different parent commit.
This is an alternative to a merge that can be neater as it doesn't require a merge commit.
Sometimes when we see "rebase your work" we just mean make sure your changes are built on top of the latest. This could be done by merging in the latest, or by rebasing onto the latest.

# Pushing and pulling

Intuitive commands - push your commits to somebody else, or pull their commits down to you.
Can be done directly between any two repos
Very often done to a "golden repository"
Golden repo is just another git repo that we have decided is the central one. Our SW golden repo is the one in bitbucket, so when we push and pull, it's almost always from bitbucket in order to share changes with the rest of the team.
This is functionally almost the same as merging between branches locally, except the branches are remote branches
Demonstrate this by setting up a github repository and pushing to it.

# Pull requests

Pull requests are a collaborative web-based feature layered on top of git and provided by services such as Bitbucket.
Gives us a web based workflow and an opportunity to perform review, run automated tests, etc.

# Tagging

Lastly tagging, tagging is super easy.
While a branch is a moving pointer to a commit, a tag is a permanent pointer to a commit.
This is commonly used for release tags, so a tag such as v10.2.5.1 is permanently points to a particular commit
We also use the act of tagging to trigger a deployment to production

# Questions!

Any?
