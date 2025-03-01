# 🚀 Commit Message Guide  

A standardized approach to writing clear and meaningful Git commit messages.  
This guide enhances collaboration, simplifies project management, and enables automated changelog generation.  

---

## 📌 Why Use Standardized Commits?  

✅ **Better Communication** – Write messages that both humans and machines can understand.  
✅ **Project Clarity** – Track changes by type (e.g., features, fixes, docs) and scope (e.g., component, module).  
✅ **Automated Workflows** – Enable semantic versioning and auto-generated changelogs.  
✅ **Team Alignment** – Reduce ambiguity in collaborative environments.  

---

## 🛠️ Getting Started  

### **Basic Workflow**  

1. **Stage Changes**  
   ```bash
   git add <files>
   git add .  # Stage all changes
   ```

2. **Commit with Message**  
   ```bash
   git commit -m "type(scope): description"
   ```

   **Example**:  
   ```bash
   git commit -m "feat(auth): add password reset endpoint"
   ```

3. **Push to Remote**  
   ```bash
   git push origin <branch-name>
   ```

---

## 📝 Commit Structure  

```plaintext
type(scope): description  # Required
<BLANK LINE>
body                      # Optional
<BLANK LINE>
footer                    # Optional (e.g., for breaking changes)
```

---

## 🔍 Key Components  

- **Type** – The purpose of the change (e.g., `feat`, `fix`, `docs`).  
- **Scope (Optional)** – The module or component affected (e.g., `api`, `button`).  
- **Description** – A short, imperative summary (“add” vs. “added”).  
- **Body/Footer** – Additional details, breaking changes, or issue links.  

---

## 🔖 Commit Types  

| **Type**   | **Purpose**                                      | **Example**                          |  
|------------|--------------------------------------------------|--------------------------------------|  
| **feat**   | Introduces a new feature                        | `feat(profile): add dark mode`       |  
| **fix**    | Fixes a bug                                     | `fix(login): handle 404 errors`      |  
| **docs**   | Updates documentation                           | `docs: update API guidelines`        |  
| **style**  | Formatting, no code logic changes               | `style: format CSS indentation`      |  
| **refactor** | Improves code structure, no behavior change    | `refactor: simplify auth logic`      |  
| **perf**   | Enhances performance                            | `perf(db): optimize queries`         |  
| **test**   | Adds or updates tests                           | `test: add login unit tests`         |  
| **build**  | Changes build system or dependencies            | `build: update Webpack config`       |  
| **ci**     | Updates CI/CD pipeline                          | `ci: fix GitHub Actions workflow`    |  
| **revert** | Reverts a previous commit                       | `revert: remove experimental API`    |  
| **design** | UI/UX changes                                   | `design(button): update hover effect`|  
| **eod**    | Work-in-progress backup at the end of the day    | `eod: WIP user dashboard layout`     |  

---

## 🌟 Best Practices  

✅ **Use Imperative Mood**  
   - Write `"fix"` instead of `"fixed"` or `"fixes"`.  

✅ **Keep It Short**  
   - Limit subject lines to 50 characters. Use the body for details.  

✅ **Reference Issues**  
   - Include Jira/GitHub issue references:  
     ```bash
     git commit -m "feat: user profile [PROJ-42]"
     ```

✅ **Indicate Breaking Changes**  
   - Add `!` after the type/scope and explain in the footer:  
     ```bash
     git commit -m "feat(api)!: remove deprecated endpoints"
     ```

✅ **Use Multi-Line Commits for Detailed Changes**  
   - Run `git commit` without `-m` to open the editor.  

---

## 🌙 End-of-Day (EOD) Commits  

For backing up work-in-progress code:  
```bash
git commit -m "eod: WIP user dashboard layout [PROJ-15]"
git push origin <branch-name>
```

---

## 🎫 Integrating with Jira/Tickets  

Include the ticket ID + title directly:  
```bash
git commit -m "[PROJ-123] fix(payment): resolve currency rounding error"
```

---


## 📂 Repository Details  

**Project**: commit-style-sheet  
**Developers**: Waleed  



