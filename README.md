# TOOLS-IN-DATA-SCIENCE-PROJECT-1

# Using the GitHub API, scrape all users in the city of Singapore with over 100 followers, and their repositories.

users.csv:  Use the SAME values as in the API response. For booleans, use true and false and empty strings for null.

repositories.csv:  Use the SAME values as in the API response. For booleans, use true and false and empty strings for null.

# users.csv has following information about each user in Singapore with over 100 followers, with fields:

login: Their Github user ID

name: Their full name

company: The company they work at. Clean up company names. At least make sure:
They're trimmed of whitespace
Leading @ symbol is stripped (Note: ONLY the first one is stripped)
They are converted to UPPERCASE

location: The city they are in

email: Their email address

hireable: Whether they are open to being hired

bio: A short bio about them

public_repos: The number of public repositories they have

followers: The number of followers they have

following: The number of people they are following

created_at: When they joined Github

# repositories.csv has these users' public repositories. For each user in users.csv, fetch up to the 500 most recently pushed repositories, with fields:

login: The Github user ID (login) of the owner, which, BTW, is not directly in the API response.

full_name: Full name of the repository

created_at: When the repository was created

stargazers_count: Number of stars the repository has

watchers_count: Number of watchers the repository has

language: The programming language the repository is written in

has_projects: Whether the repository has projects enabled

has_wiki: Whether the repository has a wiki

license_name: Name of the license the repository is under (This is under license.key).
