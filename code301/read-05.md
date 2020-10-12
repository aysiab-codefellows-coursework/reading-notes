# Reading Assignment Five
*Sections Read:*
- [Getting Started With Heroku & Node.JS](https://devcenter.heroku.com/articles/getting-started-with-nodejs)

### Quick Intro to Heroku
To get started with Heroku using your terminal and Git, you will want to install Heroku. There are different steps per your operating system. Please ger to the reading. 

Once Heroku is installed you can then use `heroku` commands in your terminal.

Within your app repository, you can call `heroku create` within your terminal to create an app on Heroku. Heroku will give your app a random name unless you pass a name as a parameter. Heroku will create a git remote called `heroku` that is associated with your local git repo. 

To deploy your code you can then call `git push heroku main`.

You will want to ensure there is at least one instance of your app running before opening it. To ensure this, run `heroku ps:scale web=1`

And to visit your live application, you can call `heroku open`

And there you have it! The bare bone basics of deploying your application through your terminal with Heroku. 