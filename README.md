# cavity1-icoFoam-Solver
Create a GitHub profile
Copy the folder cavity from $FOAM_TUTORIALS/incompressible/icoFoam/cavity/ to a local folder
Start with the copying cavity from $FOAM_TUTORIALS/incompressible/icoFoam/cavity/ to a local folder with a name cavity1



To begin, we will initialize an empty Git repository within the "cavity" folder by executing the command "git init". This command sets up the necessary files and folders to start tracking changes in the directory using Git.



After making changes to our files in the local repository, the next step is to update our local repository by committing the changes. When we commit, Git prompts us to provide information about our identity, specifically asking us to configure Git. To configure Git, we can use the "git config" command. This command allows us to set various configuration options, such as our name and email address, which will be associated with the commits we make in the repository. we configure by giving the username and email ID . 



After configuring Git, when we attempt to commit our changes, Git might display a message stating that there is "nothing to commit, working tree clean" but also indicating that there are untracked files. In this scenario, Git suggests using the "git add" command to add the untracked files to the staging area. By using the "git add" command, we specify which files we want to include in the next commit, effectively placing them in the staging area for inclusion in the repository's history.

To move files from the current folder to the staging area in Git, you can use the `git add` command. This command adds the specified files to the staging area, preparing them for the next commit.

After adding the files to the staging area, the next step is to commit the changes. The commit command in Git allows you to permanently save the changes made to the files in the local repository. The syntax for the commit command is similar to what is shown in the image.

When committing, you can provide a message to describe the changes made in the commit. This message helps in providing a concise summary of the modifications. Once the commit is executed, all the files that were added to the staging area are committed, meaning the local repository is updated with the changes.

In summary, the process involves:
1. Using `git add` to add files to the staging area.
2. Using the commit command with a descriptive message to commit the changes.
3. After the commit, the local repository reflects the updated state with the committed changes.



To update our changes to a central version control or central server, we can use the `git pull` command. However, if you encounter an error when using `git push` that states there is no destination to push, it means that you haven't created a remote repository to push your changes to.

To resolve this, you can create a repository on GitHub (or a similar platform) and establish a connection between your local repository and the remote repository. This can be done using the `git remote` command, which performs two operations simultaneously: creating a central repository in your Git configuration and linking it to the GitHub repository.

By using `git remote`, your GitHub repository becomes the central or main repository. It acts as a cloud storage for your local repository, allowing you to send your data to the central repository. This enables multiple contributors, like yourself, to access the central repository and contribute to the code.

In summary, the process involves:
1. Creating a repository on GitHub.
2. Using the `git remote` command to create a central repository in your Git configuration and connect it to the GitHub repository.
3. After this setup, you can push your changes to the remote repository on GitHub, which serves as the central version control system, enabling collaboration with other contributors.



As per  the below image you can create gitHub repository.



Now that we have created a remote repository on GitHub and have an existing local repository, we can transfer the data from our local repository to the main/central repository on GitHub. To accomplish this, we need to configure our local repository to use the "main" branch as the primary branch. Then, we can push our changes to the remote repository's main branch using the `git push` command.

When creating a repository on GitHub, the platform provides instructions and commands for setting up the remote repository. These commands are typically displayed in a highlighted area, guiding users through the process. These commands usually include steps like initializing the local repository, adding the remote repository as the "origin," setting the main branch, and pushing the changes.

In summary, the process involves:
1. Setting the local repository's branch to "main" as the primary branch.
2. Using the `git push` command to push the local repository's changes to the remote repository's main branch.
3. The specific commands required to accomplish this are usually displayed when creating a repository on GitHub.

By following these steps, we can transfer the data from our local repository to the main/central repository on GitHub, ensuring that our changes are synchronized and accessible to other contributors.



Then, after typing git push, a login and password prompt appears.We must enter both GitHub's login and password. However, it indicates that support for password authentication was terminated on August 13 due to a mistake. It requests that you use your personal access token rather than your password. The image below shows the exact same thing.



To make our push successful, we must now generate a personal access token and enter it in place of the password.To create a token, navigate to GitHub, select Settings, then select Developer Settings. From there, select Personal Access Tokens. After creating a new token, a token link will be generated; you must copy it and paste it in the place of the password for pushing.You can see that a token has been produced in the image below.



By using a personal access token as the password during the push operation, you can successfully push your changes. Upon executing `git status`, you will observe that your branch is up to date with the central repository on GitHub.



Upon refreshing the GitHub repository, you will find that the files used in Git have been successfully transferred from the local repository to the central repository on GitHub.



