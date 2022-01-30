# HOWTO

This is a guide for working with [Lacuna V3](https://lacunalab.org) website.

You will need to setup and install all the respositories for your machine.

# Overview

```
REPOSITORIES
============

eze-legacy = database gui app
lacuna-media = images & photos
lacuna-v3 = the static website

NB: EACH MUST BE IN SAME ROOT FOLDER
```

# Prerequisites

Using a terminal, you must have the following installed:

```
PREREQS
=======

GIT = normal git usage
NODE.JS = nvm is recommended
PNPM = alternative to npm
```

# Installation

```
CLONE
=====

git clone git@github.com:LacunaLab/lacuna-media.git
git clone git@github.com:LacunaLab/lacuna-v3.git
git clone git@github.com:LacunaLab/eze-legacy.git
```

There will now be 3 folders side-by-side called **lacuna media**, **lacuna-v3**, **eze-legacy**:

```
INSTALL DEPENDENCIES
====================

cd lacuna-media && pnpm i && cd ../
cd lacuna-v3 && pnpm i && cd ../
cd eze-legacy && pnpm i && cd ../
```

# Edit Website

Each time you want to add something to the website, you will need to start up the servers.

You will need **two terminals open** - one for the *backend* and one for the *frontend*:

```
IN 1ST TERMINAL (PORT 5000)
===========================

cd eze-legacy
pnpm run dev

IN 2ND TERMINAL (PORT 8888)
===========================

cd lacuna-v3
pnpm run dev
```

You can now view **backend** in [localhost:5000](http://localhost:5000) and **frontend** in [localhost:8888](http://localhost:8888)

Inside the **frontned** is a GUI for adding and editing data.

*You will be able to see your changes immediately at [localhost:8888](http://localhost:8888)**

# Make It Live

Once you are **100% happy with the changes** visible in [localhost:8888](http://localhost:8888), you can build and push a new version online.

```
BUILD
=====

cd lacuna-v3
pnpm run build

```

