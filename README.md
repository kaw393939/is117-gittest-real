# Git Test - 30 Minutes

## Do This Pattern 15 Times

```bash
git checkout -b question-01
# Write answer in answers/question-01.md
git add answers/question-01.md
git commit -m "docs: answer question 1"
git checkout main
git merge question-01
```

Change to question-02, question-03, etc.

---

## The 15 Questions

1. What does git status do?
2. What is git add vs git commit?
3. What is a Git branch?
4. What does git merge do?
5. What is git pull vs git push?
6. What does pwd do?
7. How do you use cd? Show 3 ways.
8. What does ls -la show?
9. How do you create a directory?
10. What are absolute vs relative paths?
11. How do you create an empty file?
12. What is cp vs mv?
13. Why is rm -rf dangerous?
14. What does cat do?
15. How do you view last 20 lines of a file?

---

## Commit Rules

Start with: docs: or chore: or fix:

Example: docs: answer question 5

---

## Grading

- 20 pts: 15+ commits
- 25 pts: Correct prefixes
- 20 pts: 15 branches
- 15 pts: Branches merged
- 15 pts: All files exist
- 5 pts: Files have content

---

## Start

```bash
mkdir answers
git add answers/
git commit -m "chore: create answers directory"
```

Then repeat the pattern 15 times.

---

## You Can Use Google/ChatGPT

We grade Git workflow, not answers!

---

## Push When Done

```bash
git push origin main
git push --all
```
