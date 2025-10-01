# Question 2: Explain the difference between `git add` and `git commit`.

## Answer

`git add` stages changes for commit - it tells Git which changes you want to include in the next commit. Think of it as preparing items to be photographed.

`git commit` actually saves those staged changes to your local repository with a message. It's like taking the photograph and saving it permanently.

## Example

```bash
git add file.txt         # Stage the file
git commit -m "docs: add file"  # Save it with a message
```

You must `git add` before you can `git commit`.