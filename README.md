## Blood Lords Campaign
A repo for ongoing player notes of the Pathfinder 2E Blood Lords campaign.

## Setup for Notetakers
TBD. Goal: Use Obsidian with GitHub plugin.

Instructions based on https://habr.com/en/articles/883678/

### Configure Git
1. Create a github account
2. Install git on your computer
3. Setup ssh to allow github actions without logging in each time
	1. In the git terminal, type `ssh-keygen -t ed25519 -C "your_email@example.com"`
	2. Use the default values; it will create a new .ssh directory and key files
	3. Use this command to display the SSH key `cat ~/.ssh/id_ed25519.pub` and copy the full key
	4. Go to https://github.com/settings/keys and add the SSH key you copied
4. Clone this repo with ssh
	1. Open your git terminal and navigate to the folder where you want these notes stored.
	2. Run this command: `git clone git@github.com:blomquistr/pathfinder-2e-blood-lords.git`

If you clone the repo with https, you'll have to enter your password/PAT (Personal Access Token) each time to login.
### Configure Obsidian
1. Download Obsidian: 
2. Run Obsidian and 'Open folder as vault'. Select the folder created when cloning the repo (i.e. your chosen location /pathfinder-2e-blood-lords)
3. Add the git plugin for Obsidian
	1. Turn on community plugins
	2. Browse for 'Git' plugin and enable
4. Configure the Obsidian git plugin
	1. Auto commit-and-sync interval: 10 minutes (until we prove otherwise)
	2. Enable "Pull on Startup"

You can access git commands via the Obsidian command palette (Ctrl + P). A common command to make sure your latest edits are saved off-schedule would be "Git: commit-and-sync".