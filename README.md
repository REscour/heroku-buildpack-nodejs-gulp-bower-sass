Heroku Buildpack for node, gulp, bower & sass
========================================

Usage
-----

- Set your Heroku app's buildpack URL to `https://github.com/davidmfoley/heroku-buildpack-nodejs-gulp-bower.git`. To be safe, you should really fork this and use your fork's URL.
- Run `heroku config:set NODE_ENV=production` to set your environment to `production` (or any other name)
- Add a gulp task called `heroku:production` (same as NODE_ENV) that builds your app
- Add a single line `Procfile` to the root to serve the app via node:

```
web: node [path/to/your/root/script.js]
```


Credits
-------

Forked from [heroku-buildpack-nodejs-gulp-bower](https://github.com/davidmfoley/heroku-buildpack-nodejs-gulp-bower).
