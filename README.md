# **Lab Work Summary**

## **Lab 1 – Document Review and Version Control with Git/GitHub**

**Objective:** Practice review-based testing of documentation using Git collaboration features.

**What you did:**

1. Created a short **User Manual** (`user_manual.md`) for the Student Attendance System in Markdown format.
2. Pushed it to a GitHub repository for version control.
3. Assigned **two classmates as reviewers** via Pull Requests (PRs).
4. Received comments on:

   * Clarity and completeness
   * Formatting and terminology consistency
5. Merged reviewed documents after incorporating suggestions.

**How you did it:**

* Used VS Code / any text editor to write `user_manual.md`.

* Initialized a Git repository:

  ```bash
  git init
  git add user_manual.md
  git commit -m "Initial user manual"
  git branch -M main
  git remote add origin <GitHub_repo_URL>
  git push -u origin main
  ```

* Created Pull Requests on GitHub and assigned reviewers.

* Reviewed and merged PRs after incorporating feedback.

---

## **Lab 2 – Automated Documentation Quality Check**

**Objective:** Apply automated spelling and grammar testing using Vale.

**What you did:**

1. Installed **Vale** locally for checking grammar, spelling, and style.
2. Configured Vale using `.vale.ini` and the `Styles` folder.
3. Ran Vale on the documentation file (`user_manual.md`).
4. Fixed all identified errors (spelling, grammar, style).
5. Committed the corrected documentation to GitHub.

**How you did it:**

* Installed Vale:

  ```bash
  wget https://github.com/errata-ai/vale/releases/download/v2.28.3/Vale_2.28.3_Linux_64-bit.tar.gz
  tar -xvzf Vale_2.28.3_Linux_64-bit.tar.gz
  sudo mv Vale /usr/local/bin/
  vale --version
  ```

* Created `.vale.ini`:

  ```ini
  StylesPath = Styles
  MinAlertLevel = suggestion
  [*.md]
  BasedOnStyles = Vale
  ```

* Downloaded Vale styles:

  ```bash
  mkdir Styles
  cd Styles
  git clone https://github.com/errata-ai/Styles.git .
  ```

* Introduced intentional spelling mistakes in `user_manual.md` and ran Vale:

  ```bash
  vale user_manual.md
  ```

* Fixed issues like:

  * `attendace → attendance`
  * `simultaniously → simultaneously`
  * `passd → password`
  * `upto → up to`

* Committed corrected file:

  ```bash
  git add user_manual.md
  git commit -m "Fix spelling, grammar, and style issues using Vale"
  git push
  ```

---

## **Lab 3 – Collaborative Document Writing**

**Objective:** Test documentation in real-time collaboration mode.

**What you did:**

1. Created a **Test Plan** document (`test_plan.md`) for the Student Attendance System.
2. Collaborated with a classmate using **HackMD / CodeCollab / Google Docs**.
3. Observed version conflicts, real-time edits, and automatic merging.
4. Exported the final version of the document.
5. Pushed the final document to GitHub.

**How you did it:**

* Created `test_plan.md` with sections:

  * Objective
  * Scope
  * Test Environment
  * Test Cases (login, attendance, reports, notifications, user management)
  * Version control observations
  * Notes
* Shared the document link with a classmate for co-editing.
* Recorded observations:

  * Real-time updates work instantly.
  * Conflicts are handled automatically; last edit is applied.
  * Version history allows reverting unwanted changes.
* Exported the final Markdown file and pushed it:

  ```bash
  git add test_plan.md
  git commit -m "Add final Test Plan document"
  git push
  ```

---

### ✅ **Summary Table**

| Lab   | Task Completed                                                | Tools Used                | Outcome                                          |
| ----- | ------------------------------------------------------------- | ------------------------- | ------------------------------------------------ |
| Lab 1 | Created User Manual, reviewed via PRs, merged                 | Git, GitHub               | Document reviewed collaboratively                |
| Lab 2 | Automated grammar and spelling check, fixed errors            | Vale                      | `user_manual.md` polished and Vale-approved      |
| Lab 3 | Co-edited Test Plan, exported final version, pushed to GitHub | HackMD / CodeCollab / Git | Final collaborative document versioned in GitHub |
