# Question 5: What is the difference between `git pull` and `git push`?

## Answer

`git pull` downloads changes FROM a remote repository (like GitHub) TO your local computer. It's getting the latest updates from others.

`git push` uploads your local commits FROM your computer TO the remote repository (like GitHub). It's sharing your changes with others.

## Example

```bash
git pull origin main   # Get latest changes from GitHub
# Make some changes locally...
git commit -m "docs: update readme"
git push origin main   # Send your changes to GitHub
```

Think of it as: pull = download, push = upload.