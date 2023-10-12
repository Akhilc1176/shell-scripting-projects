GitHub User List Shell Script
This shell script allows you to retrieve a list of users without needing to log in to a GitHub repository. It leverages GitHub's API to gather the list of contributors or collaborators for a specified repository.

Prerequisites
Before using this script, you need to ensure you have the following dependencies installed on your system:

cURL: The script uses cURL to make API requests to GitHub. You can install cURL by following the instructions on the cURL website.

GitHub Personal Access Token: To authenticate with the GitHub API, you will need a personal access token. You can generate a token by following GitHub's Personal Access Token documentation.

Git: To make sure you have the latest information, you should also have Git installed on your system. You can install Git from git-scm.com.

Installation
Clone this repository or download the github_user_list.sh script to your local machine.

bash
Copy code
git clone https://github.com/yourusername/github-user-list-script.git
Make the script executable.

bash
Copy code
chmod +x github_user_list.sh
Edit the script to add your GitHub Personal Access Token. Replace YOUR_ACCESS_TOKEN with your actual token.

bash
Copy code
ACCESS_TOKEN="YOUR_ACCESS_TOKEN"
Usage
You can use the script as follows:

bash
Copy code
./github_user_list.sh <repository_owner> <repository_name>
Replace <repository_owner> with the owner or organization of the GitHub repository, and <repository_name> with the name of the repository.

For example, if you want to get the list of users for the "octocat/Spoon-Knife" repository, you would run:

bash
Copy code
./github_user_list.sh octocat Spoon-Knife
The script will then make an API request to GitHub and display the list of users who have contributed to or are collaborators on the specified repository.

Notes
This script only provides a list of users. It does not reveal sensitive user information.
Be cautious when sharing or storing your GitHub Personal Access Token. Treat it like a password.
