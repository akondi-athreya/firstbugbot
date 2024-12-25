
# FirstBugBot

A Twitter bot that tweets GitHub issues labeled ‘Good First Bug’ to encourage contributions to open-source projects.

# Overview

FirstBugBot is a Twitter bot designed to automate the posting of GitHub issues tagged with ‘Good First Bug’. These are ideal issues for beginners in open-source contributing. The bot fetches open issues from GitHub, ensures they haven’t already been tweeted, and then posts them to Twitter.

# Features
	1.	Automated Issue Fetching:
	    •	Fetches GitHub issues labeled ‘Good First Bug’ using the GitHub API.
	    •	Filters out previously tweeted issues using Firebase for storage.
	2.	Tweet Scheduling:
	    •	Posts a set of tweets with random variations to Twitter.
	    •	Ensures no more than 100 tweets are sent in a single batch.
	    •	Tweets are staggered every 15 minutes to avoid overwhelming the Twitter API.
	3.	Persistence:
	    •	Utilizes Firebase Realtime Database to track and store tweeted issue IDs.
	    •	Ensures no duplicate tweets for the same issue.



# Usage
1.	Clone the repository:
	```bash
	git clone https://github.com/yourusername/FirstBugBot.git
	cd FirstBugBot
	```


2.	Install required packages:

	```bash
	npm install
	```

3.	Create a .env file with the 
following environment variables:

	```bash
	FIREBASE_APIKEY=your_firebase_api_key
	FIREBASE_AUTHDOMAIN=your_firebase_auth_domain
	FIREBASE_DATABASEURL=your_firebase_database_url
	FIREBASE_PROJECTID=your_firebase_project_id
	FIREBASE_STORAGEBUCKET=your_firebase_storage_bucket
	FIREBASE_MESSAGINGSENDERID=your_firebase_messaging_sender_id
	TWITTER_CONSUMER_KEY=your_twitter_consumer_key
	TWITTER_CONSUMER_SECRET=your_twitter_consumer_secret
	TWITTER_ACCESS_TOKEN=your_twitter_access_token
	TWITTER_ACCESS_TOKEN_SECRET=your_twitter_access_token_secret
	```

4.	Run the script:

	```bash
	npm start
	```


# Contribution

Feel free to contribute by reporting issues, submitting bug fixes, or adding new features!

