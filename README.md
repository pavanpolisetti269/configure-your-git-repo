# Set Global Git Configuration
To configure your Git username and email for the global configuration, which applies to all repositories on your system, you can use the following commands. This is useful if you want to set your identity once and have it used for all your Git activities.
## Open your terminal and run these commands:
### Set Global Username:
	git config --global user.name "Your Name"
### Set Global Email:
	git config --global user.email youremail@example.com
### Example Usage:
#### For example, if your name is John Doe and your email is john.doe@example.com, you would use:
	git config --global user.name "John Doe"
	git config --global user.email john.doe@example.com
### Verifying Global Configuration:
#### To verify that your global configuration has been set correctly, you can list the configuration settings:
	git config --list --global

# Setting Local Git Configuration
If you want to set the Git configuration for a specific repository only, instead of globally, you can use the --local option. This is useful for temporary or project-specific configurations.

### Open the terminal and navigate to your project directory:
Navigate to Your Project Directory => "cd /path/to/your/project"
### Set Local Configuration:
#### Use the --local option with git config to set the username and email for this specific repository:
	git config --local user.name "Your Local Name"
	git config --local user.email "youremail@localdomain.com"
### Verifying Local Configuration:
#### To verify the configuration has been set locally, you can list all the configuration settings:
	git config --list --local



# Steps to commit and push to Github from VSCode:

### 1. Initialize local repository :
 	git init
### 2. Add the files to be tracked by git:
 	git add .
### 3. Commit the changes: 
	git commit -m "your message here"
### 4. Add Origin: 
	git remote add origin <git-repo-link.git>

### 5. Pull repository:
	git pull --allow-unrelated-histories (repository link)  main(branch name)

### 6. Push to github: 
	git push -u origin master

## additional commands:
### 1)To terminate the connection with the github repository
	git merge --abort
### 2)If you want to temporarily store your changes without committing them: 
	git stash
### Force Push (if necessary): If you still encounter issues and are sure about your changes, you can force push: 
 	git push -f origin main
