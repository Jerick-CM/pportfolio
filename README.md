# portfolio app

## Test Website

```bash
    # install dependencies
    https://nuxt-app-frontend.herokuapp.com/

```

```bash
  # heroku commands for deployment
    heroku login
    heroku create APPNAME
    heroku buildpacks:set heroku/nodejs
    heroku config:set NODE_ENV=production
    heroku config:set NPM_CONFIG_PRODUCTION=false
    heroku config:set HOST=0.0.0.0

    add packege.json
      "scripts": {
        "heroku-postbuild": "npm run build"
      }

  cli

  git add .
  git commit -m "add nuxt for heroku"
  git push heroku
  
```

## Test Website

```bash
    # install dependencies
   

```
