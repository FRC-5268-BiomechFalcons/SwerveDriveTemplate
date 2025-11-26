# 5268 SwerveDriveTemplate

A swerve drive template based on [REVrobotics MAXSwerve Template](https://github.com/REVrobotics/MAXSwerve-Java-Template).

The goal of this template is to have some baseline functionality that will be commonly reused year to year.

# Getting Started

Below are the steps neccessary to set up this repository and start contributing!

## Installing Locally

This is a good option if you have a computer you can download all the tools on, like a Windows laptop.

1. Start by [installing WPILib](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html) for your PC if you haven't already. This comes with VSCode and all the tools neccessary to build the robot code.
2. Open the "2025 WPILib VS Code" application.
3. Clone this repository which will download the code locally to your machine. There are a couple options for this step:
    * Use VS Code's command palette (ctrl+shift+p) to run the "Git: Clone" command and follow the prompts. Search for `FRC-5268-BiomechFalcons/SwerveDriveTemplate`.
    * Follow [this article](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) from GitHub to clone using all the usual ways that GitHub supports.
4. Open the folder in VS Code if you haven't already, and you are ready to start developing!

## Using a Codespace

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/FRC-5268-BiomechFalcons/SwerveDriveTemplate)

If you are not able to download the WPILib tools or would prefer not to, this option can help you write code all in your favorite browser. Read more about codespaces [here](https://docs.github.com/en/codespaces). Our project has a default codespace devcontainer configuration defined [here](https://github.com/FRC-5268-BiomechFalcons/SwerveDriveTemplate/blob/main/.devcontainer/devcontainer.json) that will come with all the development tools you will need pre-installed.

There are some notable differences here compared to installing all the tools locally:

1. The development container runs Linux. This means that the default terminal will be [bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)).
2. The VS Code extension for WPILib does not allow for installation in this environment, so you won't have access to the usual command palette options from WPILib. For example, instead of doing `WPILib: Build Robot Code`, you will have to go to the terminal and execute `./gradlew build`.

## Branching Strategy

If you aren't familiar with branches, GitHub has a great article [about branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches).

This project has [branch protection](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches) on main. This is generally used to improve overall code quality and stability on this branch. For this project specifically, we have a minimum number of reviews required and the [Java CI action](https://github.com/FRC-5268-BiomechFalcons/SwerveDriveTemplate/actions/workflows/gradle-ci.yml) (which builds the robot code) needs to pass successfully before merging a pull request into main.

In order to actually merge code into main, you'll need to create a feature branch for your development and create a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) into the main branch when it is ready for review. I'm going to list the steps with the associated command you can run in the command line, but feel free to use the integrated VS Code source control tab if you are more comfortable with a GUI. If you don't have git installed on your system, go [here](https://git-scm.com/install/) and do that now.

In more detail, that process looks like:

1. `git checkout main` to checkout the main branch locally.
2. `git pull` to fetch all the updates from upstream main.
3. `git branch feature-name` to create a new local branch for "feature name".
4. `git checkout feature-name` to checkout the branch that you just created.
5. Write the code to implement the feature!
6. `git add --all` to stage all your changes, this adds all the modifications you made to the index.
7. `git commit` this will create a commit with all the changes staged in your index. This will open a new tab in your text editor and let you add a name and description to your commit. Once this tab is saved and closed, the command will finish.
8. `git push` will push your feature-name branch and the new commit you just made up to github.
9. [Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) from your feature-name branch into main, give it a good name and description, and add some reviewers!
10. If you have any changes to make to address reviewer comments, do step 5-8 again. The pull request should update automatically once you push an update to the branch.


