# Node Knockout Quickstart

Hello, Node Knockout hackers!

Seven years ago, before I ran Heroku's Node.js platform, I started learning node when [a friend](https://github.com/aheckmann) convinced me to join his team in the first Node Knockout.
We submitted an awesome, ambitious entry that was [riddled with bugs](https://github.com/aheckmann/Nodal-Kombat):

![Learning Node](https://pbs.twimg.com/media/DNzVMB3W4AAfg5v.jpg:large)

I entered the next year, and the next year, and didn't place until year three, but I had an amazing experience every time.
If I were to give one piece of advice, it would be:
*scope your design to what you think you can accomplish in 8 hours.*
Then, you might have a shot at finishing mostly-bug-free in 48.

Of course, it can be helpful to start from a known-good reference.
So I've put together this extremely minimal quick-start with instructions to take you from zero
to "Hello, world," with some ideas about where you might go afterwards.
If you find yourself stuck early on, this is a known-good point from which you can get un-stuck.

# Deploying

```
$ heroku create
$ git push heroku master
$ heroku open
$ heroku logs --tail
```

# Developing locally

```
$ npm install
$ npm run dev
```
