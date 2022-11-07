Bionics Docs
============

This repo contains documenation for FIRST Robotics Team 4909 the Billerica Bionics.

We attempt to document our processes and machine tools.

This repo can be built into a static website using [Hugo](https://gohugo.io)

## Prerequisites
These are needed to successfully modify and test the site.

### Submodules
Be sure to clone the repository with submodules.
```bash
git clone --recursive git@github.com:TechplexEngineer/bionics-docs.git
```
If you've already cloned, you can fetch the submodules with
```bash
git submodule update --init
```
### Hugo
Hugo is needed to build the site. Follow the [quickstart guide here](https://gohugo.io/getting-started/quick-start/).

## Local Testing
Hugo has a fantastic local development server.
```bash
hugo server
```

## Deploy
The site is deployed with Netlify, with netlify CMS support.

## Check for broken Links
```bash
muffet -i http://localhost:1313 -e http://localhost:1313/admin/\# http://localhost:1313/
```
Using: https://github.com/raviqqe/muffet

