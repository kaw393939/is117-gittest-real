# Linux Command Guide – In-Class Test (30 min)# TinyTools Calculator – In-Class Test (30 min)



## Scenario## Scenario

You've just been hired as a **Junior Documentation Specialist** at **TechStart Academy**, a coding bootcamp that teaches beginners how to use Linux. Your manager needs you to create a **beginner-friendly Linux command reference guide** using professional Git workflow and Markdown formatting.You’ve joined **TinyTools, Inc.** Deliver a production-ready **Python Calculator** library with four operations:



Your first assignment:- **add**, **subtract**, **multiply**, **divide**  

- Create a well-organized guide covering **basic Linux commands** (file operations, navigation, text viewing, and system info)- **Divide by zero must raise `ZeroDivisionError`.**

- Use **proper Markdown formatting** (headers, lists, code blocks, tables)

- Follow **professional Git workflow** with atomic commitsYour team enforces professional workflow:  

- Build the documentation **incrementally** with clear commit history- **Brand-new repo**  

- **Atomic commits** with required prefixes  

Your manager emphasizes:  - Pass **linting**  

- "We need to see your work progress through Git commits"- All **tests** must pass  

- "Each section should be added in its own commit"- **100% test coverage** required  

- "Use professional commit message prefixes so we can track documentation changes"

---

---

## Required Repo Layout

## Required Repo Layout```

```

README.mdREADME.md

docs/requirements.txt

  navigation.mdsrc/

  file-operations.mdtests/

  text-commands.md

  system-info.md````

```

---

---

## Commit Rules

## Commit Rules- Every commit message **must** start with one of:  

- Every commit message **must** start with one of:    - `chore:` — setup/config/docs  

  - `docs:` — adding or updating documentation content  - `feature:` — new functionality **and its tests**  

  - `chore:` — setup, configuration, or project structure  - `fix:` — bug fix or correcting a test  

  - `fix:` — correcting errors or improving existing content

- **Atomic history**:

- **Atomic commits**:  - Each calculator function (**add, subtract, multiply, divide**) must be delivered in **its own commit**, with the tests **and** the implementation together.  

  - Each documentation file should be added in **its own commit**  - Do **not** put multiple functions in one commit.  

  - Each major content addition gets **its own commit**  - Do **not** split one function across multiple commits.

  - Do **not** put multiple unrelated changes in one commit

  - Do **not** split one logical addition across multiple commits- **Minimum 8 commits** required (more is fine; do not squash).



- **Minimum 8 commits** required (more is fine; do not squash)### Example Commit Timeline

1. `chore: initialize repo with README and requirements`

### Example Commit Timeline2. `chore: add project skeleton (src, tests) and setup notes`

1. `chore: initialize repository with README template`3. `chore: document how to run lint/tests in README`

2. `chore: create docs directory structure`4. `feature: implement add() with unit tests`

3. `docs: add navigation commands guide`5. `feature: implement subtract() with unit tests`

4. `docs: add file operations guide`6. `feature: implement multiply() with unit tests`

5. `docs: add text viewing commands guide`7. `feature: implement divide() with unit tests including divide-by-zero`

6. `docs: add system information commands guide`8. `chore: add coverage command and enforce 100% in README`

7. `docs: add table of contents to README`9. *(if needed)* `fix: correct edge case in subtract() test`

8. `docs: add examples and tips section`10. *(if needed)* `fix: address pylint error in calculator module`

9. *(if needed)* `fix: correct mkdir command syntax in file-operations.md`

10. *(if needed)* `docs: add additional examples to navigation.md`---



---## Local Commands (before pushing)

```bash

## Content Requirements# Install dependencies

pip install -r requirements.txt

### Each Guide File Must Include:

1. **Header** (level 1 or 2)# Lint (must be clean)

2. **Command list** with descriptionspylint --errors-only src

3. **Code blocks** showing command syntax

4. **Examples** of actual usage# Run tests

5. **Tips or warnings** (using blockquotes or emphasis)PYTHONPATH=src pytest tests -v

PYTHONPATH=src pytest --pylint src -v

### Markdown Elements You Must Use:

- Headers (`#`, `##`, `###`)# Coverage (must be 100%)

- Lists (bulleted or numbered)PYTHONPATH=src coverage run -m pytest tests

- Code blocks with triple backtickscoverage report --fail-under=100

- Inline code with single backticks````

- **Bold** or *italic* text for emphasis

- Tables (at least one)---

- Blockquotes (optional but recommended)

## How Grading Works

---

Your repository is graded entirely by the **GitHub Actions workflow** in `.github/workflows/ci.yml`.

## Commands to DocumentIf any step fails, you lose points for that category.



### Navigation Commands (navigation.md)### Rubric (100 pts total)

- `pwd` - print working directory

- `cd` - change directory| # | CI Job / Step         | Requirement                                                   | Points | Pass                                    | Fail                 |

- `ls` - list directory contents| - | --------------------- | ------------------------------------------------------------- | -----: | --------------------------------------- | -------------------- |

| 1 | **Commit Policy**     | ≥ 8 commits                                                   |     20 | CI shows “Commit count requirement met” | Fewer than 8 commits |

### File Operations (file-operations.md)| 2 | **Commit Policy**     | All commit messages start with `chore:` / `feature:` / `fix:` |     20 | All messages valid                      | Any message invalid  |

- `mkdir` - make directory| 3 | **Project Structure** | `README.md`, `requirements.txt`, `src/`, `tests/` present     |     10 | All present                             | Any missing          |

- `touch` - create empty file| 4 | **Lint Check**        | `pylint --errors-only src` clean                              |     15 | No errors                               | Any error            |

- `cp` - copy files/directories| 5 | **Pytest-Pylint**     | `pytest --pylint src -v` passes                               |      5 | Pass                                    | Fail                 |

- `mv` - move or rename files| 6 | **Unit Tests**        | `pytest tests -v` passes                                      |     15 | All tests pass                          | Any fail             |

- `rm` - remove files/directories| 7 | **Coverage**          | `coverage report --fail-under=100` shows 100%                 |     15 | Exactly 100%                            | < 100%               |



### Text Commands (text-commands.md)**Total = 100 points**

- `cat` - display file contents

- `less` - view file with pagination---

- `head` - show first lines of file

- `tail` - show last lines of file## Submission



### System Info (system-info.md)* Push to GitHub/GitLab and share the repo URL **OR** upload a zip including `.git` history.

- `whoami` - current username* Your **last commit** must be before the 30-minute deadline.

- `hostname` - computer name
- `date` - current date/time
- `uname` - system information

---

## How Grading Works

Your repository is graded entirely by the **GitHub Actions workflow** in `.github/workflows/ci.yml`.
If any step fails, you lose points for that category.

### Rubric (100 pts total)

| # | Category              | Requirement                                                | Points | Pass                                    | Fail                 |
|---|-----------------------|------------------------------------------------------------|-------:|-----------------------------------------|----------------------|
| 1 | **Commit Count**      | ≥ 8 commits                                                |     15 | CI shows "Commit count requirement met" | Fewer than 8 commits |
| 2 | **Commit Messages**   | All commits start with `docs:`, `chore:`, or `fix:`        |     20 | All messages valid                      | Any message invalid  |
| 3 | **File Structure**    | All required files present                                 |     15 | All files exist                         | Any file missing     |
| 4 | **Markdown Validity** | All .md files have valid syntax                            |     15 | No markdown errors                      | Syntax errors found  |
| 5 | **Required Elements** | Headers, lists, code blocks, tables present                |     15 | All elements found                      | Missing elements     |
| 6 | **Content Quality**   | Each guide has descriptions and examples                   |     10 | Content meets standards                 | Incomplete content   |
| 7 | **Link Validity**     | All internal links work (if any)                           |     10 | No broken links                         | Broken links found   |

**Total = 100 points**

---

## Getting Started

1. **Clone or initialize your repository**
   ```bash
   git clone <your-repo-url>
   cd <repo-name>
   ```

2. **Create the structure**
   ```bash
   mkdir docs
   touch docs/navigation.md docs/file-operations.md docs/text-commands.md docs/system-info.md
   ```

3. **Make atomic commits as you add content**
   ```bash
   git add <files>
   git commit -m "docs: add navigation commands guide"
   git push
   ```

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
