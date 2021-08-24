---
title: Truffle | Installation
layout: docs.hbs
---
## Node installation under Linux
Make sure you're in the right path before installing truffle by doing the follwing steps:

1. Check if you're in the right node path:
```
which node
```
Output:
```
/home/user/.nvm/versions/node/v14.17.5/bin/node
```

2. If you need to update node to a new version. The preferred way is to use Node Version Manager on Linux and Mac OS X for a better developer experience by using this command:

```
nvm use 14
```

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

## Common errors in Linux or Mac OS X 

If you run into a config error please follow the following steps:
1. Validate the path:

```
which node
```
If your path is the follow:
```
usr/bin/node
```
Then you have to correct the Node path so when you install truffle it won't give you a permission error. Update the path or update the version of node by using NVM:

3. To correct this issue do the following:

Install nvm:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```
4. Next confirm where nvm is installed to:
```
command -v nvm
```
The output should return nvm:
```
nvm
```
5. Next would to install node by using nvm:
```
nvm install 14 
```
Now you can use node version 14 by doing:

```
nvm use 14
```
This will install node in the correct path. So when you run global node commands it will install in the right path instead of going through linux config files.

## Useful nvm commands

1. List the versions you have on your computer:
```
nvm ls
```
Output: 
```
->     v14.17.5
         system
default -> 14 (-> v14.17.5)
node -> stable (-> v14.17.5) (default)
stable -> 14.17 (-> v14.17.5) (default)
iojs -> N/A (default)
unstable -> N/A (default)
lts/* -> lts/fermium (-> v14.17.5)
lts/argon -> v4.9.1 (-> N/A)
lts/boron -> v6.17.1 (-> N/A)
lts/carbon -> v8.17.0 (-> N/A)
lts/dubnium -> v10.24.1 (-> N/A)
lts/erbium -> v12.22.5 (-> N/A)
lts/fermium -> v14.17.5
```

2. To use nvm to install the latest npm:
```
nvm install-latest npm
```

