---
title: Truffle | Installation
layout: docs.hbs
---
## Prerequisite for linux
Make sure you're in the right path before installing truffle by doing the follwing steps or it's going to give an error while trying to install on linux.

1. Check if you're in the right node path:
```
which node
```
2. If the path is:
```
usr/bin/node
```
Then you have to correct the path so when you install truffle it won't give you a permission error.

Example of the correct path:
```
/home/user/.nvm/versions/node/v14.17.5/bin/node
```
3. To correct this issue do the following:

Install nvm:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```
4. Next confirm where nvm is installed to:
```
command -v nvm
```
5. Next would to install node by using nvm:
```
nvm use 14
```
This will install node in the correct path. So when you run global node commands it will install in the right path instead of going through linux config files.

6. Once node is install properly in linux then you can run the following command in installation.

# Installation

If node is in the right path then simply run:
```bash
npm install -g truffle
```

## Requirements

* NodeJS v8.9.4 or later
* Windows, Linux or Mac OS X

Truffle also requires that you have a running Ethereum client which supports the standard JSON RPC API (which is nearly all of them). There are many to choose from, and some better than others for development. We'll discuss them in detail in the [Choosing an Ethereum client](/docs/getting_started/client) section.

## Recommendations for Windows

If you're running Truffle on Windows, you may encounter some naming conflicts that could prevent Truffle from executing properly. Please see [the section on resolving naming conflicts](/docs/advanced/configuration#resolving-naming-conflicts-on-windows) for solutions.
