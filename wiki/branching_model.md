# Branching Model

A Git branching model defines your [branching strategy](https://www.perforce.com/blog/vcs/best-branching-strategies-high-velocity-development) in Git. It determines when and how developers make changes and commit them back to your codebase.

Using a Git branching model can expedite the process of delivering feedback to developers. [Git hosting](https://www.perforce.com/git-hosting) solutions don’t come with a branching model out of the box. These Git branching models are branching patterns designed to help overcome challenges. But with Git, you have to build it!

## **Branch types**

There are several types of branches that are frequently used in software development. This section explains what each branch type is for, and the typical prefix convention for each branch type.

### **Development branch**

Usually the integration branch for feature work and is often the default branch or a named branch. For pull request workflows, the branch where new feature branches are targeted.

- `dev`

### **Production branch**

Used for deploying a release. Branches from, and merges back into, the development branch. In a Gitflow-based workflow it is used to prepare for a new production release.

- `main`

### **Feature branch**

Used for specific feature work or improvements. Generally branches from, and merges back into, the development branch, using pull requests.
They should have the following prefix `ft/`

- `ft/{FEATURE_NAME}`

### **Hotfix branch**

Used to quickly fix a Production branch without interrupting changes in the development branch. In a Gitflow-based workflow, changes are usually merged into the production and development branches.

- `ht/{BUG_NAME}`

### **Bugfix**

This branch is used to fix bugs which might be more intensive when it comes to the amount of changes to be done.  \
They should start with the prefix `bg/`

- `bg/{BUG_NAME}`

### **Release**

Branch used for release tasks and long-term maintenance versions. They are branched from the development branch and then merged into the production branch. \
They should start with this prefix `rl/`

- `rl/{VERSION}`
