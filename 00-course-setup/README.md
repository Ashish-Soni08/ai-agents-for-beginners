# Course Setup

## Introduction

This lesson will cover how to run the code samples of this course.

## Requirements

- A GitHub Account
- Python 3.12+

## Clone or Fork this Repo

To begin, please clone or fork the GitHub Repository. This will make your own verrsion of the course material so that you can run, test and tweak the code!

This can be done by clicking link to [fork the repo](https://github.com/microsoft/ai-agents-for-beginners/fork).

You should now have your own forked version of this course like below:

![Forked Repo](./images/forked-repo.png)

## Retrieve Your GitHub Personal Access Token (PAT)

Currently this course use the Github Models Marketplace to offer free access to Large Language Models(LLMs) that will be used to create AI Agents.

To access this service, you will need to create a GitHub Personal Access Token.

This can be done by going to your [Personal Access Tokens settings](https://github.com/settings/personal-access-tokens) in your GitHub Account.

Select the `Fine-grained tokens` options on the left side of your screen.

Then select `Generate new token`.

![Generate Token](./images/generate-token.png)

Copy your new token that you have just created. You will now add this to your `.env` file included in this course. 

## Add this to your Environment Variables 

To create your `.env` file run the below command in your terminal:

```bash
cp .env.example .env
```

This will copy the example file and create a `.env` in your directory.

Open that file and paste the token you created into the `GITHUB_TOKEN=` field of the .env file. 

## Environment Setup

```bash
python -V
# Output(Python Version) -> Python 3.12.1
```

```bash
# create a virtual environment
python -m venv ai-agents
```

```bash
# Install the required Python packages.
pip install -r requirements.txt
```
