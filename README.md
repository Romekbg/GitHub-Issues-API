# GitHub-Issues-API
GitHub Issues API

## Overview
This project demonstrates how to interact with the GitHub API using Postman. It includes examples of GET, POST, and PATCH requests to manage GitHub issues, labels, and repositories.

### Table of Contents
Overview
Prerequisites
Environment Setup
Project Structure
API Endpoints
  GitHub Issues
  GitHub Labels
  GitHub Repositories
Usage
  How to Run the Collection
Contributing
License

#### Prerequisites
To run the Postman collection and interact with the GitHub API, you will need:

Postman installed (latest version).
A GitHub account.
A GitHub Personal Access Token with the appropriate permissions (to interact with repositories and issues).

#### Environment Setup
1. **Postman Environment Variables**: The Postman collection uses the following environment variables:
    {{host}}: API base URL, typically set to https://api.github.com.
    {{user}}: Your GitHub username.
    {{repo}}: The name of the GitHub repository where you want to create/manage issues.
2. **Authorization**: In Postman, use the **Bearer Token** for authorization.
Set the token value as your GitHub Personal Access Token (with necessary permissions).

**#### Project Structure**
Here’s a summary of the main API calls in the collection:

GitHub Labels:

GET: Fetch labels for an issue from a specific repository.
GitHub Issues:

GET: Fetch details of an existing issue.
POST: Create a new issue in a GitHub repository.
PATCH: Modify an existing issue.
GitHub Repos:

GET: Fetch details of a GitHub repository.

**#### API Endpoints**

**GitHub Issues**
  **GET Non-existing issue**: Fetches details of a non-existing issue to demonstrate error handling.
  **GET Single issue**: Fetches the details of a specific issue using its ID.
  **POST Create issue**: Creates a new issue in the specified GitHub repository.
  **PATCH Create issue Copy**: Updates an existing issue.
  
**GitHub Labels**
  **GET GitHub Labels**: Fetches labels associated with a specific issue in a repository.
  
**GitHub Repositories**
  **GET GitHub Repos**: Retrieves details of the specified repository.


**#### Usage**

**How to Run the Collection**
1. Clone the repository to your local machine:

git clone https://github.com/your-username/your-repo.git

2. Open **Postman** and import the collection (SoftUni Demo as seen in the screenshot).

3. Make sure the **Postman environment** is configured with your GitHub credentials and repository details.

4. Run the requests in the following order for better understanding:

 Start by fetching repository details using the GET GitHub Repos request.
 Create a new issue using POST Create issue.
 Fetch issue details or labels with the respective GET requests.
 Modify an issue using PATCH Create issue Copy.


**#### Contributing**

Contributions are welcome! Feel free to open an issue or submit a pull request with any improvements or additional features you think would be helpful.

**#### License**

This project is licensed under the MIT License.
  
