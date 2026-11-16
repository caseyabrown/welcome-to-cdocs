---
layout: page
title: Add a Markdown file to a GitHub repository
permalink: /writing-samples/add-a-markdown-file-to-a-github-repository/
---

# Add a Markdown file to a GitHub repository

Markdown is a lightweight markup language that works well for [docs-as-code](https://docs.google.com/document/u/0/d/11_-3KGdzb1rm6viVDQnLqlYNArSOvAL9RYFoaQwlUhY/edit) workflows. You can use a GitHub repository to store your Markdown files (`.md`), then use git and Github for version control. This enables you to work simultaneously with other writers, while ensuring that you are not overwriting each other’s content. 

View this article to learn how to add your Markdown file to a GitHub repository. 

## Prerequisites

Before reading this article, you must have the following:

* A [GitHub](https://github.com/) account
* Access to the GitHub repository used to manage and publish your documentation
* An SSH key added to your SSH agent (see [Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent))
* Your preferred terminal (such as [iTerm2](https://iterm2.com/) or [Ghostty](https://ghostty.org/))
* [Install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to use developer tools
* Your preferred integrated development environment (IDE) (such as [Visual Studio Code](https://code.visualstudio.com/) or [Cursor](https://cursor.com/))
* A Markdown file

## On this page

* [Step 1. Clone a GitHub repository](#step-1-clone-a-github-repository)
* [Step 2. Create a branch to add your Markdown file](#step-2-create-a-branch-to-add-your-markdown-file)
* [Step 3. Create and merge your pull request in GitHub](#step-3-create-and-merge-your-pull-request-in-github)

## Step 1. Clone a GitHub repository

First, you must clone the GitHub repository and place it in a folder on your desktop. It is recommended to place the cloned repository in your `Documents` folder, as described in the following steps:

1. Open your preferred terminal.
2. Change the directory to your `Documents` folder:

   ```
   cd Documents/
   ```

3. Clone the repository:

   ```
   git clone GITHUB_URL
   ```

    **Note**: Replace `GITHUB_URL` with the link you copied from your GitHub repository. For example: `git clone git@github.com:org/microservices-repo.git`. See [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) for more information.

A message appears in your terminal to indicate when cloning is complete.

## Step 2. Create a branch to add your Markdown file 

Now that your GitHub repository is cloned, you can add your Markdown file to the repository using git. Complete the following steps:

1. Open your preferred terminal.
2. Change the directory to the location of your cloned repository:

   ```
   cd Documents/REPOSITORY_NAME
   ```

    **Note**: Replace `REPOSITORY_NAME` with the name of the cloned folder in Step 1. For example: `cd Documents/microservices-repo`

3. Locate the main branch in the repository:

   ```
   git checkout main
   ```

4. Pull down all updates since you were last in the folder:

   ```
   git pull
   ```

    The command line interface (CLI) in the terminal shows which changes were made since you were last in the folder, or shows that your local version of the repository is already up to date.

5. Create a new branch:

   ```
   git checkout -b BRANCH_NAME 
   ```

   **Note**: Replace `BRANCH_NAME` with a unique name (without spacing) for this change. For example: `git checkout -b cbrown/update-articlex`

6. Open your IDE and switch to your local branch. For example, see [Switch between branches](https://code.visualstudio.com/docs/sourcecontrol/branches-worktrees#_switch-between-branches) if you’re using Visual Studio Code.
7. Drag and drop your Markdown file to your `/docs` folder. 
8. Return to your terminal and add the changes to your local branch:
   
   ```
   git add .
   ```
  
   **Note:** No messages appear in the command line interface after you press **Enter**.

9. Add a description to the change you’re about to make:

   ```
   git commit -m "COMMIT_MESSAGE"
   ```
   **Note**: Replace `COMMIT_MESSAGE` with your description of the change. For example: `git commit -m "Added updates to article X"`

10. Push the changes to the remote branch in GitHub:

   ```
   git push origin BRANCH_NAME
   ```

   **Note**: Replace `BRANCH_NAME` with the same name associated with this change. For example: `git push origin cbrown/update-articlex`

Your changes are pushed to the remote branch and a GitHub link appears in your terminal.

## Step 3. Create and merge your pull request in GitHub

Now that you created the remote branch, you must create a pull request for your teammates to review the changes. After your pull request is approved, you can merge your branch into the `main` branch. Complete the following steps in GitHub: 

1. Copy the URL that appears in your terminal and paste it in your web browser. This is your pull request in GitHub.
2. Click **Create Pull Request**.
3. (Optional) Click the following tabs to view more about the pull request:
    * **Commits**—See which changes are being merged in this branch.
    * **Files Changed**—See the exact files that were changed.
4. Click **Merge pull request**. 
5. Click **Confirm merge**.

Your new article now appears in the GitHub repository. 

## Next steps

* See <span style="text-decoration:underline;">Verify the article</span> to confirm that it appears in your documentation set.
* View [Troubleshooting commits](https://docs.github.com/en/pull-requests/how-tos/commit-changes/troubleshooting-commits) for common commit issues.