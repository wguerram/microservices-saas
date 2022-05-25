<p><img src="./images/microservices-saas-logo.jpg" width="450"></p>

[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

# Microservices SaaS

Use this boilerplate to speed up your next SaaS deployment using NodeJS Microservices 🔥 🚀
<br/>
<br/>

This project was generated using [Nx](https://nx.dev).

🔎 **Smart, Fast and Extensible Build System**

## Adding capabilities to your workspace

Nx supports many plugins which add capabilities for developing different types of applications and different tools.

These capabilities include generating applications, libraries, etc as well as the devtools to test, and build projects as well.

Below are our core plugins:

- [React](https://reactjs.org)
  - `npm install --save-dev @nrwl/react`
- Web (no framework frontends)
  - `npm install --save-dev @nrwl/web`
- [Angular](https://angular.io)
  - `npm install --save-dev @nrwl/angular`
- [Nest](https://nestjs.com)
  - `npm install --save-dev @nrwl/nest`
- [Express](https://expressjs.com)
  - `npm install --save-dev @nrwl/express`
- [Node](https://nodejs.org)
  - `npm install --save-dev @nrwl/node`

There are also many [community plugins](https://nx.dev/community) you could add.

## Generate an application

Run `nx g @nrwl/react:app my-app` to generate an application.

> You can use any of the plugins above to generate applications as well.

When using Nx, you can create multiple applications and libraries in the same workspace.

## Generate a library

Run `nx g @nrwl/react:lib my-lib` to generate a library.

> You can also use any of the plugins above to generate libraries as well.

Libraries are shareable across libraries and applications. They can be imported from `@microservices-saas/mylib`.

## Development server

Run `nx serve my-app` for a dev server. Navigate to http://localhost:4200/. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `nx g @nrwl/react:component my-component --project=my-app` to generate a new component.

## Build

Run `nx build my-app` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `nx test my-app` to execute the unit tests via [Jest](https://jestjs.io).

Run `nx affected:test` to execute the unit tests affected by a change.

## Running end-to-end tests

Run `nx e2e my-app` to execute the end-to-end tests via [Cypress](https://www.cypress.io).

Run `nx affected:e2e` to execute the end-to-end tests affected by a change.

## Understand your workspace

Run `nx graph` to see a diagram of the dependencies of your projects.

## Further help

Visit the [Nx Documentation](https://nx.dev) to learn more.

## Branching & Merging strategy

GitHub flow

Create a branch from main

git commit will prompt for conventional commits

rebase your branch before requesting a pull request.

Because you'll be rebasing only one developer should work in a branch.

Commands sequence:

Putting aliases on the side of each command

```
# Create a branch
git checkout main  # git co main
git pull
git checkout -b my-branch  # git nb my-branch

# Make changes and do commits

# First change
git commit  # git c

# Optional push your changes
git push --set-upstream-to origin my-branch

#Second change
git commit  # git c

# Optional push your changes
git push  # git p

# When you're ready to merge do a rebase
git fetch & git rebase origin/main # git rom

# In case of conflicts, fix them and stage files modified
git add filename

git rebase --continue

git commit  # git c

# Push force latest changes, this will rewrite history in the remote. That's why no more than one developer should work on the same branch.
git push --force origin my-branch

# Create a pull request in github
# my-branch will be deleted from remote automatically after merging into main.

# Update your local main branch
git checkout main  # git co main
git pull

# Delete your local copy
git branch -D my-branch  # git del my-branch

```
