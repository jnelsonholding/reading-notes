### Class 05 Reading Notes

## Heroku

Heroku allows live updating and deployment of an app. Starting with `heroku create`, a dev simply creates an app that is tied to their local git repository.

To start an instance of the app, all that is needed is scaling it up with `heroku ps:scale web=1`. And to visit the new site, open it with `heroku open`. To scale it back down, us `heroku ps:scale web=1`. Easy peasy!

To keep an eye on the logs, use `heroku logs --tail`.

Heroku uses a Procfile to determine what processes are added to its routing stack. For example, if heroku is using node on an index.js file, the Procfile would have `web: node index.js`.

The command `heroku local web` allows a dev to run an instance on their localhost.

Heroku also has the ability to use addons (modules). To retrieve and addon, enter `heroku addons:create <nameOfAddonHere>`. And follow it with an open command: `heroku addons:open <nameOfAddonHere>`.

To access a terminal command line for heroku, you can open up a shell using `heroku run bash`.

And to add a postgresql database to your app, enter `heroku addons:create heroku-postgresql:hobby-dev` and go through heroku's steps to set up and deploy.

[Return to table of contents](../README.md)
