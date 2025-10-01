# Question 3: What is a branch in Git and why would you create one?

## Answer

A branch in Git is a separate line of development. It's like creating a copy of your project where you can make changes without affecting the main code.

You create branches to:
- Work on new features without breaking the main code
- Experiment safely
- Collaborate with others without conflicts
- Organize different versions of your work

## Example

```bash
git checkout -b new-feature    # Create and switch to new branch
# Make changes...
git checkout main              # Switch back to main
git merge new-feature          # Merge changes in
```