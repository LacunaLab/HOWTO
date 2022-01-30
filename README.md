# HOWTO (Add Stuff To The Website)

You must first setup and install all the respositories for your machine. They are organised like so:

```
REPOSITORIES
============

eze-legacy = database gui app
lacuna-media = images & photos
lacuna-v3 = the static website

NB: EACH MUST BE IN SAME ROOT FOLDER
```

# Prerequisites

You will need to use a terminal and have the following installed:

```
PREREQS
=======

GIT = normal git usage
NODE.JS = nvm is recommended
PNPM = alternative to npm
```

# Installation

When working on the website, you will need **two terminals open** - one for the *backend* and one for the *frontend*.

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

Now we will run in development:

```
IN 1ST TERMINAL
===============

cd eze-legacy
pnpm run dev

IN 2ND TERMINAL
===============

cd eze-legacy
pnpm run dev
```

You can now view **backend** in [localhost:3000
