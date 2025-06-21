# ALXprodev-advanced_git

## Project Overview
This repository, `ALXprodev-advanced_git`, is created to demonstrate and practice the GitFlow workflow as part of an advanced Git exercise. The project initializes a Git repository with GitFlow, setting up the `main` and `develop` branches, and serves as a foundation for further development using GitFlow conventions.

## Repository Setup
The repository has been initialized with the following steps:
1. Created an empty repository on GitHub named `ALXprodev-advanced_git`.
2. Cloned the repository locally.
3. Created and pushed the `develop` branch.
4. Initialized GitFlow with default settings using `git flow init -d`.
5. Added an initial `README.md` file to document the project.

## GitFlow Workflow
This project follows the **GitFlow** branching model, which includes:
- **main**: Represents the production-ready codebase.
- **develop**: Contains the latest development changes for the next release.
- **feature/***: Used for developing new features (branched from `develop`).
- **release/***: Prepares code for production (branched from `develop`, merged into `main` and `develop`).
- **hotfix/***: Quick fixes for production issues (branched from `main`, merged back into `main` and `develop`).
- **support/***: Optional branches for maintaining older versions.

## Getting Started
### Prerequisites
- Git installed on your local machine.
- GitFlow installed (`sudo apt-get install git-flow` for Ubuntu, `brew install git-flow` for macOS, or equivalent for your OS).
- A GitHub account and access to the `ALXprodev-advanced_git` repository.

### Setup Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/ALXprodev-advanced_git.git
   cd ALXprodev-advanced_git
   ```
2. **Initialize GitFlow** (if not already done):
   ```bash
   git flow init -d
   ```
   Accept default branch names and prefixes by pressing Enter.

3. **Verify branches**:
   ```bash
   git branch
   ```
   You should see `main` and `develop` branches.

### Contributing
To contribute to this project:
1. Create a feature branch from `develop`:
   ```bash
   git flow feature start <feature-name>
   ```
2. Make changes, commit, and push:
   ```bash
   git add .
   git commit -m "Describe your changes"
   git push origin feature/<feature-name>
   ```
3. Finish the feature and merge it into `develop`:
   ```bash
   git flow feature finish <feature-name>
   ```

