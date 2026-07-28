# Automated Github Organization and Team Invites
> Quickly host a webpage to allow people to click and receive an invite to your Github Organization and a selected team.

### Features

* Validates submitted Github usernames
* Links in your Github Organization's avatar/image
* Lightweight
* Auto-invite to a team inside the organization

### How to use it?
*Example commands with Ubuntu*

**Install Prerequisites:**

```
sudo apt update
sudo gem install bundler
sudo bundle config set --local platform ruby
sudo apt install -y build-essential ruby-dev libssl-dev libxml2-dev libxslt1-dev zlib1g-dev
```

**Install dependencies:** 

```
bundle install
```

**Run Locally:**

1. Open the TEAM_NAMES file in a text editor. For each line, write a valid team name of your organization, the others are going to be intentionally ignored by this website.
2. Set ORGANIZATION_NAME to the name of the organization where the teams have been created.
3. Set GIHUB_TOKEN to your [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic).
4. Finally, execute it:

```bash
ORGANIZATION_NAME="foo" GITHUB_TOKEN="bar"  bundle exec ruby web_app.rb
```

This command will try to host a server on ```http://localhost:4567/```.

### Credits 

Thanks to [the original author](https://github.com/thundergolfer/automated-github-organization-invites) for his work.
