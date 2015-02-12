This is a template repo that other repos will be created off of.

I want to have the template_repo be a repo that has generic code.
example_repo is an example of a project that is based on the template_repo.
Basically I want to have a branch on example_repo that is linked to a branch in
the template_repo so I can fetch changes made to template_repo and merge them
into a branch in example_repo and then rebase the "master" branch of
example_repo with that "template" branch.
