# What are branches?

As a reminder, branches are used for concurrent work on different parts of a project. 
They can also reduce the risk of conflicting versions of files. 
For example, we may analyze Spanish soccer data in a branch called la liga, 
while a colleague analyzes English Premier League data in a branch called premier league.

# How to create a new branch 

When we create our repo, there will be one branch called main. 
In our repo's Code section, we can see which branch we are currently located in.
We can check how many branches our repo contains by looking at the branch icon, confirming we have one branch.'
We click on this icon if we want to create a new branch.

This opens a pop-up window. We enter a branch name, la liga. 
The name should describe the scope of what it will be used for, such as dev or testing.
We can also choose the branch source, which is what GitHub uses to create the new branch. 
As we only have main, we ignore this step. Lastly, we select Create branch.

# Why do we use branches in Github?

If we are working on a small solo project we probaly only need to use the default "main" branch. 
But if we are working on a large scale project and we are collaborating, 
we use branches to work on different project tasks simultaneously. 
This means that, generally, the main branch holds the final versions of our files. 
We only incorporate contents from other branches into main once we are finished and know there are no issues.

# How to incorporate contents from other branches on to the main one when we are finnished

GitHub offers a way to enforce rules for how we use specific branches. 
For example, we can require a pull request, which we will discuss later, before branches can be merged. 
This adds a layer of protection against bringing incorrect code into our main branch.
We can also set a rule requiring pull requests to be approved before a merge can occur, 
which may help improve code quality. We might also restrict who can delete a protected branch.

To add rules, we select the Settings tab of our repo.
We choose the Branches section.
This shows us our Default branch and has a section called Branch protection rules. We click the Add rule button.
The first step is to add a name for our rule in the Branch name pattern section, which is mandatory. We call ours protect main.
We have many options, but let's enable the two we discussed previously. We click Require a pull request before merging.
This expands the section and, by default, selects the Require approvals section. 
We can edit the required number of approvals using the dropdown menu underneath, but for now, we'll leave this as one.
Lastly, we click Create at the bottom of the page to save our new rule.
