# Ghost 0.11.0 Blogging site with static generator

Quick Start Install

<a name="getting-started">Dependencies</a>
- Install [Python 2.7](https://www.python.org/download/releases/2.7/)
- Install [Buster](https://github.com/zaki-hanafiah/buster)


Install Node.js via NVM.

Use Node v0.10.48 since this is an older version of Ghost (We only need to run it locally for CMS usage)
```bash
# curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
# nvm install 0.10.48
# nvm use 0.10.48
```

Clone :ghost:

```bash
git clone https://github.com/TryGhost/Ghost/tree/0.11
cd ghost
```

Install grunt

```bash
npm install -g grunt-cli@1.0.1
```

```bash
npm install
```

Building the site

```bash
grunt init
```

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


# Copyright & License for Ghost 0.11.0

Copyright (c) 2013-2016 Ghost Foundation - Released under the [MIT license](LICENSE).
