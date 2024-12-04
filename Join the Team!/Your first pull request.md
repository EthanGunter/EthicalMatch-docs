# Your First Pull Request
So, you want to make a contribution but don't know how. This simple step-by-step guide will take you from ground zero, all the way to making your first official pull request!

## Step 1: Fork the Docs Repository
For security reasons, you will be working on your own copy of the EthicalMatch documentation, and proposing your changes to the official repository via pull requests (PRs). We'll get to that later.
1. Simply click the **Fork** button as shown below, and a copy will get added to your GitHub account
![GitHub.com fork button](../{attachments}/GitHub%20Fork%20Button.png)
> [!Note]
> You will need to have a GitHub account for this to work. Clicking **Fork** will prompt you to create an account if you don't already have one
## Step 2: Pull the Docs to Your Computer
You can't make contributions if you don't have the source to work on!
First, you need to pull what's hosted by GitHub onto your local machine. We recommend using GitHub desktop, but there are plenty of guides online if you'd rather use the Command Line Interface.
1. [Install GitHub Desktop](https://desktop.github.com/download/) and open it
1. Click File > Options > Accounts > Sign in to GitHub.com, and follow the sign in process
1. Click File > Clone Repository > GitHub.com (default tab)
1. Under **Your repositories**, select the EthicalMatch fork that you created
	- When asked "**How are you planning to use this fork?**", select "**To contribute to the parent project**", then hit continue. This will make the future contributions easier.  

The documentation should now be downloaded to your local machine at the file path you specified!

> [!Tip]
> If you don't see your fork in the GitHub.com tab, you can clone a repo using a URL instead. You can find the link to clone your repository on github.com below: 
> ![GitHub.com cloning options](../{attachments}/GitHub%20HTTPS%20clone%20URL.png)
> You can also "Open with GitHub Desktop" as seen at the bottom of this image

## Optional: Install Obsidian for Documentation Editing
Obsidian is a text editor with extensive plugin support designed for linking knowledge (documents). It is the editor of choice for the EthicalMatch project.
1. [Download Obsidian](https://obsidian.md/download) and open it
1. Click **Open Folder as Vault**, and select the directory you cloned your fork into
1. Click **Trust author and enable plugins**
> [!Note]
> These plugins are all quality of life plugins, and choosing to use Obsidian without them won't prevent you from contributing
## Step 3: Make a Branch
Think of branches like workspaces. Each branch allows you to work on changes in isolation, without affecting any other branches. While it's technically not necessary to create a branch to create a pull request, it is highly recommended.
1. In **GitHub Desktop**, click **Current Branch** in the top center.
1. You can either select an existing branch, or you can create a new one by
    - clicking **New Branch**, giving it a name, and clicking **Create branch**
    - If your work is related to an issue, name your branch to reflect it (e.g., `#17-pull-request-guide`)
![GitHub Desktop "New branch" button](../{attachments}/GH%20Desktop%20New%20Branch.png)

> [!Warning]  
> If you're looking to address a GitHub issue, someone else might be working on it already. Make sure to check the comments of the issue and the **Assignees** section on the right sidebar so your time isn't wasted!  
> (You might try reaching out them in our [Discord](https://discord.gg/P7qfVuqMXz) to see if they'd like a hand)
## Step 4: Make and Commit Some Changes
With your branch ready, you can now make changes!
1. Open the files you want to edit in Obsidian or your preferred text editor
1. Change some stuff
1. In **GitHub Desktop**, view the **changes** tab on the left
	- Make sure you're not committing any erroneous changes that aren't related to your branch's purpose. You can just uncheck them, or right click and discard them.
1. At the bottom of the changes tab, write a summary of your work (e.g., "Fixed typos in CONTRIBUTING.md")
1. Click **Commit** to save your changes locally

> [!Tip]  
> Committing doesn't automatically upload your changes to GitHub. You'll do that in the last step.

## Step 5: Sync with the Project's Main Branch
Since it takes time to make changes, it's possible that the official repo has had some updates while you were working. In order to make sure that you're still up to date, you need to merge the upstream changes into your local version:
1. Click **Fetch Origin** to detect any changes that might have happened on the remote
1. Make sure you are on whatever branch you want to update. In the example, I'm updating **#17-pull-request-guide**
1. At the bottom of the **Current Branch** selector, click the **Choose a branch to merge…** button
1. In the popup window, select **upstream/main** 
1. Click **Create a merge commit**  
	- If the button is disabled saying that your branch is up to date, no further action is needed!
	- If you get a message saying "Cannot merge while there are changes on your branch", just click **Stash Changes**. These can easily be recovered by clicking **stashed changes** at the bottom of the **changes** tab on the left
![Selecting a branch to update from|320](../{attachments}/GH%20Desktop%20Sync%20upstream.png) ![Creating a merge commit|350](../{attachments}/GH%20Desktop%20Create%20Merge%20Commit.png)
> [!Note]
> Creating a merge commit will add a new commit for the merge, as well as a commit for every change that has happened on the upstream branch. Don't be alarmed when it says you've got 12 commits to push!
## Step 6: Submit a Pull Request
Now it's time to propose your changes to the project! If you haven't already pushed your changes, all of your changes are local, and we need them on GitHub in order to make a Pull Request (PR)
1. In **GitHub Desktop**, right of the **Current Branch** selector, click **Push Origin** to upload your changes to GitHub
1. Open the **Current Branch** dropdown, and click on the **Pull Requests** tab. Click the link that says "… **create a pull request** …"
1. Follow the prompts to submit your pull request with a brief description of your changes
1. Make sure **Allow Edits by Maintainers** is checked, then click **Create Pull Request**
    
> [!Tip]  
> PRs that point to an open GitHub Issue will be accepted far more quickly than random pull requests. If your changes address an issue, you can reference it by using GitHub's [auto-linking keywords](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/using-keywords-in-issues-and-pull-requests) (eg "fixes #13")

---

Congratulations! 🎉 You've officially submitted your first pull request. The EthicalMatch team will review your changes and get back to you soon.