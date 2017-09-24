# Brief Description

This is an NRIC Validation implementation that gets Api.ai classification JSON (i.e. a JSON output of Api.ai /query endpoint) and returns a fulfillment response.

# First Step: Creating a telegram bot via Botfather at telegram

Once obtained the token key, please keep it for for the next step.

# Second step: Setting up API.AI
1. Sign up and Sign in at API.AI
2. Create an Agent with your preferred name
3. Click on 'Integrations' and enable 'Telegram'. Enter the telegram bot's token key
4. (Optional) You can test the app by entering anything in your telegram bot
5. (Optional) Click on 'Small Talks' and enable - Please feel free to adjust the options and settings of the Small talks to your own liking

# Third step: Clone this respo

Open up your terminal and enter the following. Please do ensure you are in your preferred directory (e.g Desktop)
```
git clone https://github.com/Harrizontal/Basic-python-server-with-APIAI.git
cd Basic-python-server-with-APIAI
```

# Forth Step: Create a heroku app and deploy it

To create a heroku app, please enter the following
```
heroku create {ENTER YOUR APP NAME HERE, IT MUST BE UNIQUE}
```

After creating, please enter this:
```
git push heroku master
```
To open, please do the following first:
```
heroku ps:scale web=1
```

Then type the following to open the heroku app:
```
heroku open
```

It should open a 404 website because there is no html file in the server. However, you can do the following to check is there any connection to the server:
```
heroku logs --tail
```

# Fifth Step: Sign up a Github account
1. Sign up and Sign in at github.com
2. Create a respo with your preferred name

# Sixth Step: Download and install SourceTree (git version interface control)
Uh..just google it but remember to log in to your github account

# What does the service do?
It's a NRIC Validity fulfillment service that takes in an NRIC number where both alphabets have to be in capital letter.
The services takes the `NRIC` parameter from the action, are returns a validity status to Api.ai.

The service packs the result in the Api.ai webhook-compatible response JSON and returns it to Api.ai.
