# Empiresmod main page

The main page for [Empiresmod, a free indie RTS/FPS game](http://www.empiresmod.com/) - free open source software built with [Hugo](gohugo.io).
This repository makes it possible for anyone, not just Empiresmod developers, to improve empiresmod.com by [submitting a pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).
Hugo makes it easy to modify and view your local copy; you are expected to view and test before submitting your modification.

# Clone this repository

Scroll up, copy from the green "Clone or download" button on the right, plug that into your git GUI (e.g. [GitExtensions](https://gitextensions.github.io/)) or copy the following into a terminal window:

```
git clone git@github.com:EmpiresCommunity/website.git
```

# Install hugo

[Install hugo as described here](https://gohugo.io/getting-started/installing/), and then run:

```
hugo server -D
```

Which serves a local version from [localhost:1313](http://localhost:1313/) which you should test. 

# Deploy

You can't deploy unless the Empiresmod dev team has given you 'developer' rights on EmpiresmodCommunity. Everyone else, submit a pull request.

The `./deploy` script builds the full site using hugo, and then pushes the public/ subdirectory to this repository, git@github.com:EmpiresCommunity/website on the gh-pages branch. That serves empiresmod.com directly. We previously had a script on a DreamHost webserver that kept up to date on the gh-pages branch, and gave some advantages such as https support, which we can't get with github pages, but the code had a bug so we torched it and ran away.

Deploy uses the existing repository in public if it is already present. The advantage of that is that your upload will be smaller. However, since it always force pushes, each developer has their own version of all the commits, which means that if two developers keep pushing, the uploads they both must do to update the site become larger and larger. The way to get the best of both worlds is to periodically remove the whole public/ directory, so you don't keep uploading old commits.

# Stuck?

If you get stuck trying to follow these steps, [open an issue](https://github.com/EmpiresCommunity/website/issues/new).

