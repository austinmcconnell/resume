# Austin McConnell's Online Resume

Hello! You've found the repository for my online resume.

You can view my resume by going to [https://austinmcconnell.github.io/resume](https://austinmcconnell.github.io/resume).

This is built with [HackMyResume](https://github.com/hacksalot/HackMyResume) and uses CircleCI to build the webpage and deploy to GitHubPages. 


## Local Development

Install hackmyresume globally

```bash
npm install hackmyresume -g
```

Install project specific dependencies

```bash
npm install
```

Build resume webpage

```bash
npm build
```

## Custom jsonresume theme

To test against a custom jsonresume theme from a local repository, install that theme using a relative path 

```bash
npm install ../jsonresume-theme-austinmcconnell 
```

Test all output formats 

```bash
hackmyresume build resume.json TO out/resume.all -t node_modules/jsonresume-theme-austinmcconnell
```
