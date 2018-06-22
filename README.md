Netlify-cli
===========

Pluggable CLI for Netlify. 🎉

<!-- toc -->
* [Local Development](#local-development)
* [Commands](#commands)
<!-- tocstop -->

# Local Development

1. Clone down the repo

    ```bash
    git clone git@github.com:DavidWells/cli.git
    ```

2. Install dependencies

    ```bash
    npm install
    ```

3. Run CLI locally during development

    ```bash
    ./bin/run [command]
    ```

<!-- # Usage
usaxge  
```sh-session
$ npm install -g netlify-cli
$ netlify-cli COMMAND
running command...
$ netlify-cli (-v|--version|version)
netlify-cli/0.0.0 darwin-x64 node-v9.2.0
$ netlify-cli --help [COMMAND]
USAGE
  $ netlify-cli COMMAND
...
```
<!-- usagxestop -->

# Commands
<!-- commands -->
* [`netlify-cli functions`](#netlify-cli-functions)
* [`netlify-cli functions:build`](#netlify-cli-functionsbuild)
* [`netlify-cli functions:create`](#netlify-cli-functionscreate)
* [`netlify-cli functions:list`](#netlify-cli-functionslist)
* [`netlify-cli functions:serve`](#netlify-cli-functionsserve)
* [`netlify-cli functions:update`](#netlify-cli-functionsupdate)
* [`netlify-cli login`](#netlify-cli-login)
* [`netlify-cli logout`](#netlify-cli-logout)
* [`netlify-cli sites`](#netlify-cli-sites)
* [`netlify-cli sites:create`](#netlify-cli-sitescreate)
* [`netlify-cli sites:delete SITEID`](#netlify-cli-sitesdelete-siteid)
* [`netlify-cli sites:list`](#netlify-cli-siteslist)
* [`netlify-cli sites:update`](#netlify-cli-sitesupdate)

## `netlify-cli functions`

Manage netlify functions

```
USAGE
  $ netlify-cli functions

DESCRIPTION
  The `functions` command will help you manage the functions in this site

EXAMPLES
  $ netlify functions:create --name function-xyz --runtime nodejs
  $ netlify functions:update --name function-abc --timeout 30s
```

_See code: [src/commands/functions.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions.js)_

## `netlify-cli functions:build`

build functions locally

```
USAGE
  $ netlify-cli functions:build

OPTIONS
  -n, --name=name  name to print
```

_See code: [src/commands/functions/build.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions/build.js)_

## `netlify-cli functions:create`

create a new function locally

```
USAGE
  $ netlify-cli functions:create

OPTIONS
  -n, --name=name  name to print
```

_See code: [src/commands/functions/create.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions/create.js)_

## `netlify-cli functions:list`

list sites

```
USAGE
  $ netlify-cli functions:list

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/functions/list.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions/list.js)_

## `netlify-cli functions:serve`

serve functions locally for dev

```
USAGE
  $ netlify-cli functions:serve

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/functions/serve.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions/serve.js)_

## `netlify-cli functions:update`

update a function

```
USAGE
  $ netlify-cli functions:update

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/functions/update.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/functions/update.js)_

## `netlify-cli login`

Login to account

```
USAGE
  $ netlify-cli login
```

_See code: [src/commands/login.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/login.js)_

## `netlify-cli logout`

Logout of account

```
USAGE
  $ netlify-cli logout
```

_See code: [src/commands/logout.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/logout.js)_

## `netlify-cli sites`

Handle site operations

```
USAGE
  $ netlify-cli sites

DESCRIPTION
  The sites command will help you manage all your sites

EXAMPLES
  $ netlify sites:create -name my-new-site
  $ netlify sites:update -name my-new-site
```

_See code: [src/commands/sites.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/sites.js)_

## `netlify-cli sites:create`

create a site

```
USAGE
  $ netlify-cli sites:create

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/sites/create.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/sites/create.js)_

## `netlify-cli sites:delete SITEID`

delete a site

```
USAGE
  $ netlify-cli sites:delete SITEID

ARGUMENTS
  SITEID  Site ID to delete

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here

EXAMPLE
  $ netlify site:delete 123-432621211
```

_See code: [src/commands/sites/delete.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/sites/delete.js)_

## `netlify-cli sites:list`

list sites

```
USAGE
  $ netlify-cli sites:list

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/sites/list.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/sites/list.js)_

## `netlify-cli sites:update`

update a site

```
USAGE
  $ netlify-cli sites:update

OPTIONS
  -n, --name=name  name to print

DESCRIPTION
  ...
  Extra documentation goes here
```

_See code: [src/commands/sites/update.js](https://github.com/netlify/cli/blob/v0.0.0/src/commands/sites/update.js)_
<!-- commandsstop -->

---

**Notes from previous CLIs**

**Go CLI commands**

via https://github.com/netlify/netlifyctl

```
Available Commands:
  assets    # List assets attached to a site
  ├── add   # Add an asset to a site
  └── info  # Show information for an asset or a group of them
  deploy    # Deploy your site
  form      # List forms
  └── submissions # list form submissions
  help      # Help about any command
  init      # Configure continuous deployment
  login     # Log user in
  site      # Handle site operations
  ├── create   # create site
  └── update   # Update site settings
  version
```

**Node CLI Commands**

via https://github.com/netlify/netlify-cli

```
createSite = require("../lib/commands/create_site"),
deleteSite = require("../lib/commands/delete_site"),
deploy     = require("../lib/commands/deploy"),
publish    = require("../lib/commands/publish"),
init       = require("../lib/commands/init"),
list       = require("../lib/commands/list_sites"),
updateSite = require("../lib/commands/update_site"),
openSite   = require("../lib/commands/open"),
env        = require("../lib/commands/env"),
```

**Misc examples**

- https://github.com/feinoujc/gh-search-cli/blob/master/src/commands/code.ts#L16-L53
- https://github.com/oclif/plugin-plugins#what-is-this
