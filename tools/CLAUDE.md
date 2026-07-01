# CLAUDE.md — tools

This dataset contains information about general software tools, icluding self-hosted services, managed services, libraries and frameworks, etc.

A goal is to exclude exclude low-quality and possibly short-lived tools that may be the result of a hype cycle. Some indicators to identify such tools are: 

- Is there a Git repo? If yes, how popular is it?
- Is the description on the website overly AI focused and using buzzwords?
- Does the website put the pricing section at a relatively prominent position, is there no free tier, or does the pricing seem unreasonable (basically, inciting users to just sign up and pay without having a sufficient amount of information about the product)?
- Does the website put trust-inducing badges at prominent positions (e.g. "5 out of 5 stars", "best value", "most recommended", etc.)?
- Does the website have an About section that clearly identifies the company or organisatino behind the product (e.g. history, address, contact informatio contact information, size and background of team, etc.)?

## Giraffe computed fields

Fields that are omitted from the data files but are intended to be added in as computed fields in Giraffe:

- `github_stars`
- `github_forks`
- `github_issues`
- `github_pull_requests`
- `github_commits`
- `github_contributors`
- `github_first_commit_date`
- `github_last_commit_date`
- `github_repo_creation_date`

> Note: the computation of all the `github_*` field is dependent on the `github_url` field which is pare of the core data. For records that don't have a GitHub URL, the `github_url` field as well as all the `github_*` fields will have `"n/a"` values.

> Note: `github_repo_creation_date` (the date the repository was created on GitHub) and `github_first_commit_date` (the date of the first commit in the repository's history) are not necessarily the same. They typically coincide for repositories that were created empty and built up from scratch on GitHub, but can diverge if a Git repository with an existing history was added to a new GitHub repository.
