# Version Control

**Version Control: An Overview**

- **Definition**: Version control is a system that records changes made to files over time. It takes snapshots of files as edits are made and saves them for future reference.
- **Track Changes Feature**: Similar to the track changes feature in Microsoft Word, which tracks and allows reverting to previous edits.
- **Git**: A sophisticated version control system developed in 2005. It tracks changes on multiple files, supports collaboration, and is widely used.
- **Benefits of Version Control**:
    - **Single Updated Version**: Maintains one updated version of each file with a record of all previous versions.
    - **Change Records**: Keeps a record of who, when, and why changes were made.
    - **Conflict Management**: Ensures that simultaneous edits do not conflict, facilitating merging of multiple changes.
- **Git**:
    - **Local Copy**: Keeps a local copy of work and revisions, which can be synced with the main online repository.
    - **Collaboration**: Allows multiple people to work on the same files simultaneously without disturbing the common repository.
- **GitHub**: An online interface for Git, similar to Dropbox. It hosts files and records changes online, integrating with Git to track file versions and changes.
- **Key Terms**:
    - **Repository (Repo)**: Equivalent to a projects folder. Contains all version-controlled files and changes.
    - **Commit**: Saving edits and changes. Each commit is like a snapshot with a message explaining the changes.
    - **Push**: Updating the online repository with local edits.
    - **Pull**: Updating the local version of the repository to reflect changes made by others.
    - **Staging**: Preparing a file for commit. Allows separating file changes into different commits.
    - **Branch**: Simultaneous copies of a file. Allows working on separate versions before merging.
    - **Merge**: Combining independent edits into a single file.
    - **Conflict**: Occurs when edits are incompatible. Requires manual resolution.
    - **Clone**: Copying an existing Git repository to create a local version.
    - **Fork**: Personal copy of a repository taken from another person.
- **Best Practices**:
    - **Purposeful Commits**: Each commit should address a single issue.
    - **Descriptive Messages**: Write precise commit messages to explain changes.
    - **Regular Updates**: Frequently pull and push changes to stay current with the repository.

**Summary**: Understanding version control, Git, and GitHub is essential for managing file changes, collaborating effectively, and maintaining organized project repositories.

# GitHub ang Git

**Setting Up GitHub and Git**

1. **Creating a GitHub Account**:
    - Visit: [www.github.com](http://www.github.com/).
    - Fill in your information: Username, email, and secure password.
    - Click "Sign up for GitHub" to create your account.
    - To log in, go to [github.com](http://github.com/) and enter your credentials.
2. **Navigating GitHub**:
    - **User Settings**:
        - Click the icon with a narrow in the upper right corner to access your profile.
        - Go to "Edit Profile" to add your name, bio, and picture.
        - Explore account settings to edit your password or username.
    - **Notifications**:
        - Click the bell icon to view notifications for repositories and collaborations.
    - **Help**:
        - Click "Help" at the bottom of any page to access GitHub's help system.
    - **Creating Your First Repository**:
        - Follow the GitHub guide to create your first repository.
        - Explore your repository to view commit history and contributions.
    - **Repositories Tab**:
        - On your profile, click the "Repositories" tab to view all your repositories and their activity.
3. **Installing Git**:
    - **Windows**:
        - Go to [git-scm.com/download](http://git-scm.com/download) and download the installer.
        - Open the `.exe` file and follow the installation wizard. Accept default options unless necessary.
        - Check "Launch Git Bash" and deselect "View Release Notes" if not needed.
        - Git Bash will open for command-line use.
    - **Mac**:
        - Download the `.dmg` file from [git-scm.com](http://git-scm.com/).
        - Open the file, double-click the `.pkg` file, and follow the installation wizard, accepting defaults.
    - **Alternative Installations**: Refer to [git-scm.com](http://git-scm.com/) for other Mac installation methods.
4. **Configuring Git**:
    - Open Git Bash (Windows) or Terminal (Mac).
    - Set your Git username:
        
        ```bash
        git config --global user.name "Your Name"
        
        ```
        
    - Set your Git email (use the email associated with GitHub):
        
        ```bash
        git config --global user.email "your.email@example.com"
        
        ```
        
    - Confirm the configuration:
        
        ```bash
        git config --list
        
        ```
        
    - Exit the command line by typing `exit` and pressing enter.

**Summary**:

- You created a GitHub account, explored its interface, and created your first repository.
- You installed Git and configured it with your username and email for integration with GitHub.
- You are now prepared to link Git with RStudio and manage your projects effectively.

# Linking GitHub and R Studio

1. **Linking RStudio to Git**:
    - Open RStudio.
    - Go to **Tools** > **Global Options** > **Git/SVN**.
    - Ensure the Git executable path is correct. If not, update it to the correct directory.
    - Click **Okay** or **Apply**.
2. **Creating and Adding an RSA Key**:
    - In the **Git/SVN** tab, click **Create RSA Key**.
    - Once completed, click **Close**.
    - Click **View public key**, copy the key, and close the window.
3. **Adding the SSH Key to GitHub**:
    - Log in to [GitHub](http://github.com/).
    - Go to **Account Settings** > **SSH and GPG keys**.
    - Click **New SSH key**, paste the public key you copied from RStudio, and give it a relevant title.
    - Confirm with your GitHub password.
4. **Creating a Repository on GitHub**:
    - On GitHub, go to your **Profile** > **Repositories** > **New**.
    - Name your repository and provide a short description.
    - Click **Create Repository** and copy the repository URL.
5. **Linking the Repository to RStudio**:
    - In RStudio, go to **File** > **New Project**.
    - Select **Version Control** and choose **Git**.
    - Paste the repository URL, choose the project location, and click **Create Project**.
    - This initializes a new RStudio project linked to the GitHub repository.
6. **Creating and Committing a File in RStudio**:
    - In RStudio, go to **File** > **New File** > **R Script**.
    - Enter the following code:
        
        ```
        print("This file was created within RStudio")
        print("And now it lives on GitHub")
        
        ```
        
    - Save the file within the new project directory.
    - In the **Git** tab of the environment quadrant, check the box under **Staged** to stage your file.
    - Click on **Commit**, write a commit message, and click **Commit**.
7. **Pushing Changes to GitHub**:
    - After committing, push your changes to GitHub.
    - Go to your GitHub repository to verify that the commit has been recorded.

**Summary**:

- You’ve successfully linked RStudio with Git and GitHub.
- You created a repository on GitHub, linked it with RStudio, created a file, and managed it using Git within RStudio.
- Your changes were pushed to GitHub, completing the integration process.

# Projects under Version Control

**Linking an Existing R Project to Git and GitHub**

1. **Set Up a Local Project Not Under Version Control**:
    - Open RStudio.
    - Go to **File** > **New Project** > **New Directory** > **New Project**.
    - Name your project and ensure **Create a git repository** is **not** selected.
    - Click **Create Project**.
2. **Initialize Git for Your Existing Project**:
    - Open **Git Bash** or **Terminal**.
    - Navigate to the project directory:
        
        ```bash
        cd path/to/your/project
        
        ```
        
    - Initialize Git in this directory:
        
        ```bash
        git init
        
        ```
        
    - Add all project files to the repository:
        
        ```bash
        git add .
        
        ```
        
    - Commit the changes:
        
        ```bash
        git commit -m "Initial commit"
        
        ```
        
3. **Link Local Git Repository to GitHub**:
    - Go to [GitHub](http://github.com/) and create a new repository.
    - Name the repository the same as your R project.
    - Do **not** initialize the repository with a README, .gitignore, or license.
    - After creating the repository, you will see instructions to push an existing repository from the command line.
    - Copy and paste these commands into **Git Bash** or **Terminal** to link your local repository to GitHub:
        
        ```bash
        git remote add origin <https://github.com/yourusername/yourrepository.git>
        git branch -M main
        git push -u origin main
        
        ```
        
    - Refresh your GitHub page to confirm the repository is now linked.
4. **Verify Integration in RStudio**:
    - Reopen your project in RStudio.
    - You should now see the **Git** tab in the upper right quadrant.
    - You can use this tab to stage, commit, and push changes to GitHub.
5. **Cloning an Existing GitHub Repository**:
    - If you need to contribute to an existing project:
        - Go to **File** > **New Project** > **Version Control**.
        - Select **Git** as your version control system.
        - Enter the URL of the existing GitHub repository.
        - Choose a location on your computer to store the project files.
        - Click **Create Project**.
    - The existing files from the GitHub repository will be cloned to your local machine, and you can manage them through RStudio.

**Summary**:

- You’ve learned how to convert an existing R project to use Git for version control and link it to GitHub.
- You initialized the Git repository locally, linked it to GitHub, and verified the setup in RStudio.
- You also reviewed how to clone an existing GitHub repository to your local machine using RStudio for contributing to ongoing projects.