# Austin McConnell's Online Resume

Hello! You've found the repository for my online resume.

You can view my resume by going to [https://austinmcconnell.github.io/resume](https://austinmcconnell.github.io/resume).

This is built with [resume-cli](https://github.com/jsonresume/resume-cli) and uses CircleCI to build the webpage and deploy to GitHubPages.

## Local Development

Install project-specific version of node

```bash
nvm install $(cat .nvmrc)
```

Activate project-specific version of node

```bash
nvm use $(cat .nvmrc)
```

Install project specific dependencies

```bash
npm install
```

Build resume webpage

```bash
node_modules/.bin/resume export --format html --theme jsonresume-theme-austinmcconnell public/index.html
```

or use VS Code `Build index.html` task

## Custom jsonresume theme

To test against a custom jsonresume theme from a local repository, install that theme using a relative path

```bash
npm install ../jsonresume-theme-austinmcconnell
```
