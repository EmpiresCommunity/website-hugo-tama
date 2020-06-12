# What?

A minimal hugo website, based on the [themeless gitless introduction to hugo](https://www.ii.com/themeless-gitless-intro-hugo/), to serve as a proof of concept for features you will need in every hugo website. You can fork this repository to start your website.

Current features:

- Sass @import for [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) CSS'ing.
- A navigation bar (in `layouts/_default/baseof.html`)
- test and deploy scripts to hide the flags hugo should receive
- About & Contact pages
- Articles indexed by tag

Feel free to open a pull request if there's anything missing.

# Setup instructions:

## 1) Install extended hugo

Follow the guide at [gohugo.io/getting-started/installing/](gohugo.io/getting-started/installing/)

## 2) Clone and build 

```
git clone http://github.com/TamaMcGlinn/hugo-tutorial
cd hugo-tutorial
./test
```

## 3) View & edit cycle

That last command runs `hugo server -D` which displays a local server (hosted at [http://localhost:1313/](http://localhost:1313/)) which automatically updates if you modify the files it depends on.

## 4) Deploy

The deploy script builds the site into `public/`. Add to this script whatever you need to actually upload it to the production server.
