# Heroku Deployment
Heroku is known for making server configurations easy and painless. We can build faster and worry about the things that matter to us instead of trying to configure our own servers.

## Tools Needed
You'll need a few things to start your deployment:

* Node and npm
* Heroku Toolbelt: Windows Mac Debian 
* Ubuntu
* Git Bash


## Logging Into Heroku
This is the way we can link our local desktop to Heroku. We will authenticate from the command line so that Heroku will know that we are authorized to send applications for deployment. This is a fairly easy process.

Just type: 
```
$ heroku login
```

## Deploying Your Node App
This is a very simple process. From within the folder of your git repo, we do the following steps:

* Create a remote repository (called `heroku` as opposed to our main origin remote repository) so our application knows where to push our deployable code
* Push the repository!

## Deploying Code
Now that we have everything in order, go ahead and push to Heroku!
```
$ git push heroku master
```

