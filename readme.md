# Node Knockout Quickstart

Hello, Node Knockout hackers!

Seven years ago, before I ran Heroku's Node.js platform, I
[started learning node](https://twitter.com/HunterLoftis/status/926850031591804929)
when [a friend](https://github.com/aheckmann)
convinced me to join his team in the first Node Knockout.
We submitted an awesome, [ambitious entry](https://github.com/aheckmann/Nodal-Kombat) that was riddled with bugs.

I entered the next year, and the next year, and didn't place until year three, but I had an amazing experience every time.
Node Knockout is a great way to push yourself, to learn, to have fun, and to hang out with friends.

From my own experience, my biggest piece of advice for teams is:
*scope your design to what you think you can accomplish in 8 hours.*
Then, you might have a shot at finishing mostly-bug-free in 48.

Right behind that would be: *do not wait until the last minute to deploy your application*. Start
from something basic, get it running in production, and then push it periodically as you work on it.

It can be helpful to start from a known-good reference, so I've put together this extremely 
minimal quick-start with instructions to take you from zero
to "Hello, world," with some ideas about where you might go afterwards.
If you find yourself stuck early on, this is a known-good point from which you can get un-stuck.

If you're more comfortable with the patterns in create-react-app, there's a [documented react/node starter pack](https://github.com/heroku-examples/node-knockout-react-node-starter)	that gets you set up with a backend Node service and a static frontend React app as well.

# Getting set up

1. [Register your Node Knockout team](https://www.nodeknockout.com/).
2. [Install Node.js 8.9.1 locally](https://nodejs.org/en/download/).
3. [Install the Heroku CLI](https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up) and log in with your [free account](https://signup.heroku.com/dc).

# Creating your NKO app

First, give your app a name and pull the quick start code:

```
$ git init my-nko-idea
$ cd my-nko-idea
$ git pull https://github.com/hunterloftis/nko-quickstart.git
```

Then, create an app on Heroku and check that you get "Hello, Node Knockout:"

```
$ heroku create my-nko-idea
$ git push heroku master
$ heroku open
```

If everything looks good, set this app up as your NKO app:

```
$ git remote add origin (your node knockout github url)
$ git push origin master
```

Finally, save your app name in your [Node Knockout Team page](https://www.nodeknockout.com/team/edit).

# Developing locally

First, install dependencies:

```
$ npm install
```

Then, start your app in dev-mode, open [localhost](http://localhost:5000), and edit away:

```
$ npm start
```

# Deploying changes

To deploy updates to your app:

```
$ git commit -am 'something awesome'
$ git push heroku master
$ heroku open
```

You might also want to stream your app's logs in the background:

```
$ heroku logs --tail
```

# Leveraging the Ecosystem

I encourage you to use Heroku's ecosystem of free add-ons so you can focus entirely on what makes your app unique during the competition. I've listed a few here, but there are [many more](https://elements.heroku.com/addons):

- Data stores:
[Postgres](https://elements.heroku.com/addons/heroku-postgresql),
[Redis](https://elements.heroku.com/addons/heroku-redis),
[MongoDB](https://elements.heroku.com/addons/mongolab)
- Queues and messaging:
[AMQP](https://elements.heroku.com/addons/cloudamqp),
[Pusher](https://elements.heroku.com/addons/pusher)
- Other:
[User management](https://elements.heroku.com/addons/auth0),
[Geocoding](https://elements.heroku.com/addons/geocody),
[Video, audio, image processing](https://elements.heroku.com/addons/transloadit)
