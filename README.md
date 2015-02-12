This is a template repo that other repos will be created off of.

I want to have the template_repo be a repo that has generic code.
example_repo is an example of a project that is based on the template_repo.
Basically I want to have a branch on example_repo that is linked to a branch in
the template_repo so I can fetch changes made to template_repo and merge them
into a branch in example_repo and then rebase the "master" branch of
example_repo with that "template" branch.

In other words:
I have two repos:
* template_repo - contains common code
 * template_branch - the main branch. (not named master to avoid conflict with branches in other repos)

* example_repo - a project that uses the common code provided by template_repo
 * master - the master branch that is deployed to production
 * template_branch - linked to the template_branch in template_repo

I want to be able to pull the changes made in template_repo into a branch in example_repo, let's call it "template_branch".
Then I want to be able to rebase the "master" branch with "template_branch" to pull in the changes to common code.

