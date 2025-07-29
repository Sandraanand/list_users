# 🔐 GitHub Repo Access Checker

This shell script lists users who have **read access (pull permission)** to a specific GitHub repository using the GitHub REST API.

---

## Script Overview

The script:
- Uses the GitHub REST API to query repository collaborators
- Authenticates via your **GitHub username and Personal Access Token (PAT)**
- Filters and lists users with **read (pull)** access

---

##  Requirements

- `curl` – for making HTTP requests
- `jq` – for parsing JSON responses
- A **GitHub Personal Access Token** with `repo` or `read:org` permission

---

##  Usage

```bash
# Set your GitHub credentials as environment variables
export USERNAME=your_github_username
export TOKEN=your_personal_access_token

# Run the script with repository owner and repo name
./listuser.sh <repo_owner> <repo_name>

