# Austin McConnell's Online Resume

Hello! You've found the repository for my online resume.

You can view my resume by going to https://austinmcconnell.github.io/resume.

I use [HackMyResume](https://github.com/hacksalot/HackMyResume) and a git pre-commit hook to generate an index.html file from austinmcconnell.json which is then served via GitHubPages.

The pre-commit hook is found in the repository. You'll need to create a symlink in the .git/hooks folder with the following command

```
ln -sfv ../../pre-commit .git/hooks/
```

If you'd like more information on how I did this so you can do it too, open an issue and ask for clarification. I'm happy to help!
