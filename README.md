# Ghost 0.8.0 Blogging site with static generator

Quick Start Install

<a name="getting-started">Dependencies</a>
- Install [Python 2.7](https://www.python.org/download/releases/2.7/)
- Install [Buster](https://github.com/Misiur/buster)


Install Node.js via NVM.

```bash
# Use Node v0.10.48
```

Clone :ghost:

```bash
git clone git://github.com/tryghost/ghost.git
cd ghost
```

Install grunt. No prizes here.

```bash
npm install -g grunt-cli
```

Install Ghost. If you're running locally, use [master](https://github.com/TryGhost/Ghost/tree/master). For production, use [stable](https://github.com/TryGhost/Ghost/tree/stable). :no_entry_sign::rocket::microscope:

```bash
npm install
```

Build the things!

```bash
grunt init
```

Minify that shit for production?

```bash
grunt prod
```

Start your engines.

```bash
npm start

## running production? Add --production
```

Verify that everything is running via `npm start`, if ghost site is served and running, proceed to next steps. If there are any errors, fix them first before proceed to the steps below as we need a working Ghost CMS local setup as a pre-requisite.

# Setup Buster 
```bash
buster setup
```
* Enter github repo URL once prompted (Can be SSH or HTTPS URL)

# Generate static Ghost site
```bash
buster generate --domain=http://127.0.0.1:2368/
```

# Preview static Ghost site via Buster
```bash
buster preview
```

# Deploying Ghost to Github Pages

```bash 
buster deploy
```


# Copyright & License for Ghost 0.8.0

Copyright (c) 2013-2016 Ghost Foundation - Released under the [MIT license](LICENSE).
