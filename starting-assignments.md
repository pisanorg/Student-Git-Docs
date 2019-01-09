# Starting a New Assignment from GitHub Classroom

When you will be creating repos for GitHub classroom, you'll want to follow these steps.

## Step 0. Accept the Assignment

Your instructor will provide you with a link to the assignment. It should look
something like this: `https://classroom.github.com/a/xxxxxxx`. Open that link
in your browser.

![accept the assignment](img/authorize-github-classroom-3.PNG)

Clicking this button will create a new repo for you to work in.
This typically takes a few seconds.

![clone assignment](img/authorize-github-classroom-4.PNG)

When this is done, you'll see this confirmation page.

![clone confirmation](img/authorize-github-classroom-5.PNG)

## Step 1. Clone the repository

Open the repository link that was created for you by GitHub classroom.
This will be your private repository for working on the assignment.

![new cloned assignment screenshot](img/new-cloned-assignment.png)

If your instructor has provided a template for the assignment, you may see
that your repo already contains files. Otherwise, your repo may be empty.

Click on the green _"Clone or download"_ button.

![clone or download button](img/clone-button.png)

Make sure that this says _"Clone with HTTPS"_. If it doesn't, click the link in the top right of this pop-up.
SSH is only used if you have set up certificates, which is a topic that we will not cover in this document.

Copy the link provided in this popup.

### Linux and Mac Instructions

Open your terminal application.

Type the following to navigate to your home directory: `cd ~`.

Then, create a folder called _"Git"_ under this directory: `mkdir Git`.
This will be used to store all of your Git projects.

Navigate into this directory with: `cd Git`

You can then clone your project using: `git clone https://github.com/instructororg/yourrepohere.git`
with the link from your GitHub repository.

You will be asked for your GitHub username and password. When typing in your password, you will not see
any indicators for your password, so just hit Enter/Return when you are done.

Then, using the command `ls`, you should see a new directory for your assignment in this directory.
`cd directoryName` to it, and you should see your files there.

### Windows Instructions

Create a new folder with the name _"Git"_, under your `C:\` drive.

Open _Command Prompt_. Use the following command to navigate to that folder: `cd C:\Git`.

You can then clone your project using: `git clone https://github.com/instructororg/yourrepohere.git`
with the link from your GitHub repository.

You will be asked for your GitHub username and password. When typing in your password, you will not see
any indicators for your password, so just hit Enter/Return when you are done.

Then, open the folder `C:\Git` under File Explorer, and your files should be there.

