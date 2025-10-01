# Question 4: What does `git merge` do? Provide an example scenario.

## Answer

`git merge` combines changes from one branch into another. It takes the commits from a feature branch and integrates them into your current branch (usually main).

## Example Scenario

You're working on a new login feature:

```bash
git checkout -b login-feature  # Create feature branch
# Write code for login...
git commit -m "feat: add login form"
git checkout main              # Go back to main
git merge login-feature        # Bring login changes into main
```

Now main has all your login feature code!