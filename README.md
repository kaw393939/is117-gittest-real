# Git & Linux Command Guide - In-Class Test (30 min)# Linux Command Guide – In-Class Test (30 min)# TinyTools Calculator – In-Class Test (30 min)



## Scenario

Welcome to **TechStart Academy**! You've been hired as a Junior Developer, and your manager needs to verify you can follow professional Git workflow. Your task is to answer 15 technical questions about Git and Linux commands using **proper branch-based development workflow**.

## Scenario## Scenario

**Important:** This test evaluates your **Git workflow skills**, not memorization. You may use ChatGPT, Google, or any resources to answer questions. What matters is demonstrating professional version control practices.

You've just been hired as a **Junior Documentation Specialist** at **TechStart Academy**, a coding bootcamp that teaches beginners how to use Linux. Your manager needs you to create a **beginner-friendly Linux command reference guide** using professional Git workflow and Markdown formatting.You’ve joined **TinyTools, Inc.** Deliver a production-ready **Python Calculator** library with four operations:

---



## Your Task

Your first assignment:- **add**, **subtract**, **multiply**, **divide**  

Answer **15 questions** about Git and Linux commands. Each question must be completed on its own branch and merged back to main.

- Create a well-organized guide covering **basic Linux commands** (file operations, navigation, text viewing, and system info)- **Divide by zero must raise `ZeroDivisionError`.**

### Required Workflow (FOR EACH QUESTION):

- Use **proper Markdown formatting** (headers, lists, code blocks, tables)

1. **Create a feature branch** for the question

2. **Create/edit the answer file** - Follow **professional Git workflow** with atomic commitsYour team enforces professional workflow:  

3. **Commit with proper message prefix**

4. **Switch back to main**- Build the documentation **incrementally** with clear commit history- **Brand-new repo**  

5. **Merge the branch**

6. **Repeat for next question**- **Atomic commits** with required prefixes  



---Your manager emphasizes:  - Pass **linting**  



## Example Workflow- "We need to see your work progress through Git commits"- All **tests** must pass  



```bash- "Each section should be added in its own commit"- **100% test coverage** required  

# Question 1

git checkout -b question-01- "Use professional commit message prefixes so we can track documentation changes"

# Create and edit answers/question-01.md

git add answers/question-01.md---

git commit -m "docs: answer question 1 about pwd command"

git checkout main---

git merge question-01

## Required Repo Layout

# Question 2

git checkout -b question-02## Required Repo Layout```

# Create and edit answers/question-02.md

git add answers/question-02.md```

git commit -m "docs: answer question 2 about cd command"

git checkout mainREADME.mdREADME.md

git merge question-02

docs/requirements.txt

# Continue for all 15 questions...

```  navigation.mdsrc/



---  file-operations.mdtests/



## The 15 Questions  text-commands.md



Answer each question in a separate markdown file: `answers/question-XX.md`  system-info.md````



### Git Questions (Questions 1-5)```



**Question 1:** What does `git status` do and when would you use it?---



**Question 2:** Explain the difference between `git add` and `git commit`.---



**Question 3:** What is a branch in Git and why would you create one?## Commit Rules



**Question 4:** What does `git merge` do? Provide an example scenario.## Commit Rules- Every commit message **must** start with one of:  



**Question 5:** What is the difference between `git pull` and `git push`?- Every commit message **must** start with one of:    - `chore:` — setup/config/docs  



### Linux File Navigation (Questions 6-10)  - `docs:` — adding or updating documentation content  - `feature:` — new functionality **and its tests**  



**Question 6:** What does the `pwd` command do? Provide an example output.  - `chore:` — setup, configuration, or project structure  - `fix:` — bug fix or correcting a test  



**Question 7:** How do you change directories using the `cd` command? Show three different ways.  - `fix:` — correcting errors or improving existing content



**Question 8:** What does `ls -la` show you that `ls` alone does not?- **Atomic history**:



**Question 9:** How do you create a new directory? Provide the command and an example.- **Atomic commits**:  - Each calculator function (**add, subtract, multiply, divide**) must be delivered in **its own commit**, with the tests **and** the implementation together.  



**Question 10:** What's the difference between absolute and relative paths? Give examples.  - Each documentation file should be added in **its own commit**  - Do **not** put multiple functions in one commit.  



### Linux File Operations (Questions 11-15)  - Each major content addition gets **its own commit**  - Do **not** split one function across multiple commits.



**Question 11:** How do you create an empty file in Linux? Provide the command.  - Do **not** put multiple unrelated changes in one commit



**Question 12:** Explain the difference between `cp` and `mv` commands.  - Do **not** split one logical addition across multiple commits- **Minimum 8 commits** required (more is fine; do not squash).



**Question 13:** Why is the `rm -rf` command dangerous? How can you be safer?



**Question 14:** What does the `cat` command do? Provide an example use case.- **Minimum 8 commits** required (more is fine; do not squash)### Example Commit Timeline



**Question 15:** How would you view the last 20 lines of a log file?1. `chore: initialize repo with README and requirements`



---### Example Commit Timeline2. `chore: add project skeleton (src, tests) and setup notes`



## Commit Message Rules1. `chore: initialize repository with README template`3. `chore: document how to run lint/tests in README`



Every commit message **must** start with one of these prefixes:2. `chore: create docs directory structure`4. `feature: implement add() with unit tests`



- `docs:` — Adding or updating documentation/answers3. `docs: add navigation commands guide`5. `feature: implement subtract() with unit tests`

- `chore:` — Setup, configuration, or structural changes

- `fix:` — Correcting an error in your answer4. `docs: add file operations guide`6. `feature: implement multiply() with unit tests`



**Examples:**5. `docs: add text viewing commands guide`7. `feature: implement divide() with unit tests including divide-by-zero`

```

docs: answer question 1 about pwd command6. `docs: add system information commands guide`8. `chore: add coverage command and enforce 100% in README`

docs: answer question 2 about cd command

fix: correct git merge explanation in question 47. `docs: add table of contents to README`9. *(if needed)* `fix: correct edge case in subtract() test`

```

8. `docs: add examples and tips section`10. *(if needed)* `fix: address pylint error in calculator module`

---

9. *(if needed)* `fix: correct mkdir command syntax in file-operations.md`

## Required Repository Structure

10. *(if needed)* `docs: add additional examples to navigation.md`---

```

README.md

answers/

  question-01.md---## Local Commands (before pushing)

  question-02.md

  question-03.md```bash

  question-04.md

  question-05.md## Content Requirements# Install dependencies

  question-06.md

  question-07.mdpip install -r requirements.txt

  question-08.md

  question-09.md### Each Guide File Must Include:

  question-10.md

  question-11.md1. **Header** (level 1 or 2)# Lint (must be clean)

  question-12.md

  question-13.md2. **Command list** with descriptionspylint --errors-only src

  question-14.md

  question-15.md3. **Code blocks** showing command syntax

```

4. **Examples** of actual usage# Run tests

---

5. **Tips or warnings** (using blockquotes or emphasis)PYTHONPATH=src pytest tests -v

## Grading Rubric (100 points)

PYTHONPATH=src pytest --pylint src -v

This test is **auto-graded by GitHub Actions**. Your score is based entirely on Git workflow:

### Markdown Elements You Must Use:

| # | Requirement | Points | How It's Checked |

|---|-------------|--------|------------------|- Headers (`#`, `##`, `###`)# Coverage (must be 100%)

| 1 | **Minimum 15 commits** | 20 pts | Git history shows ≥15 commits |

| 2 | **Proper commit prefixes** | 25 pts | All commits use `docs:`, `chore:`, or `fix:` |- Lists (bulleted or numbered)PYTHONPATH=src coverage run -m pytest tests

| 3 | **15 branches created** | 20 pts | Git history shows 15 feature branches |

| 4 | **15 successful merges** | 15 pts | All branches merged to main |- Code blocks with triple backtickscoverage report --fail-under=100

| 5 | **All 15 files exist** | 15 pts | All question-XX.md files present |

| 6 | **Files have content** | 5 pts | Each file has at least 10 words |- Inline code with single backticks````



**Total: 100 points**- **Bold** or *italic* text for emphasis



---- Tables (at least one)---



## Getting Started- Blockquotes (optional but recommended)



### Step 1: Clone and Setup## How Grading Works

```bash

git clone <your-repo-url>---

cd <repo-name>

mkdir answersYour repository is graded entirely by the **GitHub Actions workflow** in `.github/workflows/ci.yml`.

git add answers/

git commit -m "chore: create answers directory"## Commands to DocumentIf any step fails, you lose points for that category.

git push

```



### Step 2: Answer Questions Using Branch Workflow### Navigation Commands (navigation.md)### Rubric (100 pts total)

Follow the example workflow above for each question.

- `pwd` - print working directory

### Step 3: Verify Your Work

```bash- `cd` - change directory| # | CI Job / Step         | Requirement                                                   | Points | Pass                                    | Fail                 |

# Check commit count

git log --oneline | wc -l- `ls` - list directory contents| - | --------------------- | ------------------------------------------------------------- | -----: | --------------------------------------- | -------------------- |



# Check branches created| 1 | **Commit Policy**     | ≥ 8 commits                                                   |     20 | CI shows “Commit count requirement met” | Fewer than 8 commits |

git branch -a

### File Operations (file-operations.md)| 2 | **Commit Policy**     | All commit messages start with `chore:` / `feature:` / `fix:` |     20 | All messages valid                      | Any message invalid  |

# Check all files exist

ls answers/- `mkdir` - make directory| 3 | **Project Structure** | `README.md`, `requirements.txt`, `src/`, `tests/` present     |     10 | All present                             | Any missing          |

```

- `touch` - create empty file| 4 | **Lint Check**        | `pylint --errors-only src` clean                              |     15 | No errors                               | Any error            |

### Step 4: Push Everything

```bash- `cp` - copy files/directories| 5 | **Pytest-Pylint**     | `pytest --pylint src -v` passes                               |      5 | Pass                                    | Fail                 |

git push origin main

git push --all  # Push all branches- `mv` - move or rename files| 6 | **Unit Tests**        | `pytest tests -v` passes                                      |     15 | All tests pass                          | Any fail             |

```

- `rm` - remove files/directories| 7 | **Coverage**          | `coverage report --fail-under=100` shows 100%                 |     15 | Exactly 100%                            | < 100%               |

---



## Tips for Success

### Text Commands (text-commands.md)**Total = 100 points**

⏰ **Time Management**

- ~2 minutes per question- `cat` - display file contents

- Create branch → answer → commit → merge

- Don't overthink answers - you can use any resources- `less` - view file with pagination---



🔄 **Git Workflow**- `head` - show first lines of file

- Keep commits atomic (one per question)

- Always merge back to main after each question- `tail` - show last lines of file## Submission

- Push frequently to avoid losing work



✅ **Answer Quality**

- Answers don't need to be long (2-4 sentences is fine)### System Info (system-info.md)* Push to GitHub/GitLab and share the repo URL **OR** upload a zip including `.git` history.

- Include command examples when relevant

- Use ChatGPT or Google - this is about Git, not memorization- `whoami` - current username* Your **last commit** must be before the 30-minute deadline.



🚨 **Common Mistakes to Avoid**- `hostname` - computer name

- Forgetting to create a branch- `date` - current date/time

- Working on main instead of feature branches- `uname` - system information

- Missing the commit message prefix

- Not merging back to main---



---## How Grading Works



## SubmissionYour repository is graded entirely by the **GitHub Actions workflow** in `.github/workflows/ci.yml`.

If any step fails, you lose points for that category.

1. **Push all commits to GitHub**

   ```bash### Rubric (100 pts total)

   git push origin main

   git push --all| # | Category              | Requirement                                                | Points | Pass                                    | Fail                 |

   ```|---|-----------------------|------------------------------------------------------------|-------:|-----------------------------------------|----------------------|

| 1 | **Commit Count**      | ≥ 8 commits                                                |     15 | CI shows "Commit count requirement met" | Fewer than 8 commits |

2. **Verify on GitHub** that you see:| 2 | **Commit Messages**   | All commits start with `docs:`, `chore:`, or `fix:`        |     20 | All messages valid                      | Any message invalid  |

   - 15+ commits| 3 | **File Structure**    | All required files present                                 |     15 | All files exist                         | Any file missing     |

   - All answer files in the `answers/` folder| 4 | **Markdown Validity** | All .md files have valid syntax                            |     15 | No markdown errors                      | Syntax errors found  |

   - Proper commit messages| 5 | **Required Elements** | Headers, lists, code blocks, tables present                |     15 | All elements found                      | Missing elements     |

| 6 | **Content Quality**   | Each guide has descriptions and examples                   |     10 | Content meets standards                 | Incomplete content   |

3. **Your last commit must be before the 30-minute deadline**| 7 | **Link Validity**     | All internal links work (if any)                           |     10 | No broken links                         | Broken links found   |



The automated grader will run immediately and show your score in the GitHub Actions tab.**Total = 100 points**



------



## Quick Reference## Getting Started



### Branch Workflow Pattern1. **Clone or initialize your repository**

```bash   ```bash

git checkout -b question-XX          # Create branch   git clone <your-repo-url>

# Edit file   cd <repo-name>

git add answers/question-XX.md       # Stage changes   ```

git commit -m "docs: answer question XX about TOPIC"

git checkout main                     # Back to main2. **Create the structure**

git merge question-XX                 # Merge branch   ```bash

```   mkdir docs

   touch docs/navigation.md docs/file-operations.md docs/text-commands.md docs/system-info.md

### Useful Git Commands   ```

```bash

git status                           # Check current state3. **Make atomic commits as you add content**

git log --oneline                    # View commit history   ```bash

git branch                           # List branches   git add <files>

git branch -a                        # List all branches including remote   git commit -m "docs: add navigation commands guide"

```   git push

   ```

Good luck! Remember: **This is a Git workflow test, not a memorization test.** 🚀

4. **Check your work locally** (optional but recommended)
   - Preview your Markdown files in VS Code or GitHub
   - Verify all files are created
   - Count your commits: `git log --oneline | wc -l`

---

## Tips for Success

- ⏰ **Time management**: Spend ~3-4 minutes per guide file
- 📝 **Start simple**: Add basic content first, enhance later if time permits
- 🔄 **Commit often**: It's better to have too many commits than too few
- ✅ **Check requirements**: Use the rubric as a checklist
- 🚀 **Push frequently**: Don't wait until the end to push all commits

---

## Submission

- Push to GitHub and share the repository URL
- Your **last commit** must be before the 30-minute deadline
- Make sure you've pushed **all commits** to the remote repository
- The automated grader will run immediately after the deadline
