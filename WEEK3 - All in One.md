# WEEK3 — Session 4: Project Proposal, Task Guides, and Edit Record

**Course:** Session 4 individual project proposal · **Author:** Cao-ops402 · **Repository:** [eighty-thousand-steamed-buns](https://github.com/Cao-ops402/eighty-thousand-steamed-buns)

This is the single-file version of the Week 3 submission: the project proposal, two task guides, the constrained edit record, and a frozen copy of the Week 2 tutorial, in the order a reader needs them.

## How this file maps to the checkpoint

| Session 4 checkpoint requirement | Where |
| --- | --- |
| A clear product, reader, platform, and task scope | Part 1, sections 1–2 |
| A README proposal and a feasible document plan | Part 1, sections 3–4 |
| A safe copy of the earlier practice tutorial | Part 5, Appendix A |
| A short tool rationale and a repository link | Part 1, sections 5–6 |
| Suggested changes and uncertain facts | Part 4 |

---

## Part 1 — Project proposal — GitHub Web Starter

*GitHub Web Starter: Three Guides for Your First Repository*

A three-page documentation set that takes a first-year student from a new GitHub account to a shared, editable repository, using only the browser.

### 1. Product, platform, and reader

| Item | Decision |
| --- | --- |
| **Product** | A documentation set of three task guides for the GitHub web interface. Each guide is 150–250 words and ends with a Result Check. |
| **Platform** | GitHub in a desktop browser: Chrome, Edge, Firefox, or Safari. No command line, no GitHub Desktop, no mobile app. |
| **Target reader** | A first-year student with a new free GitHub account, no Git experience, and English as a second language. |

#### Reader profile

The reader profile is written as constraints on the writing, not as a description of a market.

- **No Git vocabulary.** The reader knows "file" and "folder", not "commit", "branch", or "clone". Each term is defined at first use or avoided.
- **Clicks by label, not by memory.** The reader looks for the exact words on screen, so every on-screen label is bolded exactly as GitHub prints it.
- **Two tabs, one screen.** The guide sits in one tab, github.com in another. Each step must stand alone, because the reader cannot read step 4 while clicking step 1.
- **Success means first-try completion.** If the reader has to ask a classmate what to click next, the guide failed.

### 2. Task scope

Three related tasks on one ladder: **create → add → share**. Each task produces the input for the next, so the set is one project rather than three unrelated pages.

| # | Task | Guide | Status |
| --- | --- | --- | --- |
| 1 | Create a private repository with a README | Part 5, Appendix A | Done in Weeks 1–2, frozen copy |
| 2 | Add a file to that repository in the browser | Part 2 | Draft, labels sourced |
| 3 | Invite a classmate as a collaborator | Part 3 | Draft, labels sourced |

**In scope:** one repository, one file, one collaborator, all through the web interface.

**Out of scope:** Git commands, pull requests, GitHub Pages, organisations, billing, and account recovery. Each is a separate task for a different reader, and each would double the length of the set.

### 3. README proposal

The repository's `README.md` is the front door; this part is the proposal behind it. Both follow one rule: answer the reader's three questions in ten seconds.

1. **What is this?** A documentation set, not a program. The first line states the outcome, not the topic.
2. **Who is it for?** A named reader with named limits, so the writing has something to fail against.
3. **Where do I start?** The task table gives the order. A reader who only needs task 2 opens guide 2 and never reads guide 1.

The README leaves out installation steps, badges, licence text, and screenshots of the author's own account. None of them helps a first-year student click the next label.

### 4. Document plan

| Where | Purpose | Words | Verification |
| --- | --- | --- | --- |
| Part 1 (this part) | Session 4 proposal | 1,000–1,100 | Renders on GitHub; every link opens |
| Part 2 | Task 2 guide | 150–250 | Click through on a clean account; 3 result items observed |
| Part 3 | Task 3 guide | 150–250 | A classmate receives the invitation and opens the repository |
| Part 5, Appendix A | Frozen Week 2 guide | 219 | SHA-256 recorded in Part 5; text never edited |
| Part 4 | Revision record | 1,100–1,300 | Every open fact listed with a way to close it |

**Writing standard for every guide**

Seven items, from the class checklist:

1. One `#` title; `##` for sections.
2. Numbered steps, one action per step.
3. Bold every on-screen label exactly as GitHub prints it.
4. Imperative mood, verb first.
5. Short active sentences; no filler.
6. One term for one thing.
7. 150–250 words, ending with an observable Result Check.

**Order of work**

1. Draft tasks 2 and 3 to the seven items above. *Done.*
2. Click both guides through on a second, clean account and correct any label that differs. *Next.*
3. Give the drafts to one classmate; fix whichever step they stumble on.
4. Freeze the Week 2 guide, record its checksum, and stop editing it.
5. Commit each guide separately, so every label change has a readable diff.

### 5. Tool rationale

**Markdown in VS Code, with preview open.** Markdown is the format GitHub renders, so the file a reader opens is the page I write. A Word file would add a conversion step and break copy-paste of labels. Side-by-side preview catches heading-level mistakes before they reach a commit, and the Problems panel flags broken relative links between guides.

**Git and the GitHub web editor, one commit per guide.** A diff shows exactly which label changed between drafts, which is the only reliable way to keep a quoted label quoted. Uploading a finished .docx would replace the history with a single opaque file.

**`wc -w` for word count.** Counting is mechanical, so it should be done by a tool that always returns the same number. The catch: `wc -w` counts list markers and heading hashes as tokens, so the plan states the counting method once and uses it everywhere.

**GitHub Docs as the label source.** Every bolded label in guides 2 and 3 was read from a GitHub Docs page and recorded in Part 4, so any label can be traced back to its source sentence.

**Why not Word, Notion, or a wiki.** Each one renders its own page layout, and the reader would then learn that layout as well as GitHub's. The whole point of this set is that the reader learns one interface.

### 6. Repository

<https://github.com/Cao-ops402/eighty-thousand-steamed-buns>

The repository holds the documentation set, the archived practice tutorial, and the revision record. It is the only deliverable; no ZIP is needed because the whole set is versioned here.

---

## Part 2 — Guide: How to Add a File to a Repository in the Browser

Add one file to an existing repository in about two minutes, without installing anything.

### Prerequisites

- A repository you own, created with the archived Week 2 guide in Part 5, Appendix A.
- You are signed in to github.com in the same browser.

### Steps

1. **Open the repository.** Open your repository's main page on github.com.
2. **Start a new file.** Above the list of files, click the **Add file** dropdown, then choose **Create new file**.
3. **Name the file.** In the file name field, type a name and an extension, for example `notes.md`. To place the file in a folder, type the folder name and a `/` first.
4. **Write the content.** Type your text in the file contents box. Start a line with `#` to make a heading.
5. **Preview the formatting.** Click **Preview** above the text box to see the rendered file.
6. **Commit the file.** Click **Commit changes...**. In the **Commit message** field, type a short message such as `Add notes.md`. Click **Commit changes**.

### Result Check

- `notes.md` appears in the file list.
- Your commit message appears above the file list.
- Clicking `notes.md` opens the file with your text in it.

If all three items are visible, the file was added successfully.

### If a step fails

- **Commit changes** is greyed out: the file name field is empty. Type a name.

---

## Part 3 — Guide: How to Invite a Classmate to Your Repository

Give one classmate access to your private repository so they can open and edit it.

### Prerequisites

- Your own repository, already containing at least one file.
- Your classmate's GitHub username.
- A free plan. Free accounts can invite unlimited collaborators to a personal repository.

### Steps

1. **Open the repository.** Open your repository's main page on github.com.
2. **Open the settings.** Under the repository name, click **Settings**.
3. **Find collaborators.** In the **Access** section of the sidebar, click **Collaborators**.
4. **Start the invitation.** Click **Add people**.
5. **Choose the person.** In the search field, type your classmate's username, then click the matching name.
6. **Send the invitation.** Click **Add NAME to REPOSITORY**, where NAME and REPOSITORY are the values GitHub shows.
7. **Ask them to accept.** Your classmate opens the GitHub email and accepts. Access starts on acceptance, not when you send.

### Result Check

- The **Collaborators** page lists your classmate with a pending invitation until they accept.
- After they accept, your classmate opens the repository link and sees your files.
- Your classmate can reach the **Add file** dropdown and the editor.

If all three items are true, access works.

### If a step fails

- **Settings** is missing: you are not the owner. Ask the owner to invite you.
- Your classmate sees a 404 page: the invitation is still pending, or they signed in to another account.

---

## Part 4 — Constrained edit review

This is the record of one constrained editing pass over this project's draft, run against the class writing checklist. The constraints came first; the edits second; the open questions last.

### 1. Constraints held fixed

| Constraint | How it was held |
| --- | --- |
| **Product** | GitHub web starter guides. No rename, no new product, no second audience. |
| **Scope** | Three tasks, one repository, browser only: create → add → share. Nothing added outside that ladder. |
| **Verified UI labels** | Every bolded label in guides 1 and 2 is copied from a GitHub Docs page, not typed from memory. A label that could not be sourced from a page was deleted from the guide and moved to section 4 below. |

#### Label sources

| Guide | Source page | Labels taken from it |
| --- | --- | --- |
| Part 2 | GitHub Docs, *Creating new files* | **Add file**, **Create new file**, **Preview**, **Commit changes...**, "Commit message", **Commit changes** |
| Part 3 | GitHub Docs, *Inviting collaborators to a personal repository* | **Settings**, **Access**, **Collaborators**, **Add people**, **Add NAME to REPOSITORY** |

### 2. Checklist applied

The same seven items that govern the guides, from the class checklist: one `#` title with `##` sections; numbered steps, one action each; bold labels exactly as on screen; imperative mood; short active sentences without filler; one term for one thing; 150–250 words with an observable Result Check.

### 3. Suggested changes

Each row is a change I made during the revision pass. The "before" wording is kept so the reason stays checkable.

| # | Where | Before | After | Checklist item | Why |
| --- | --- | --- | --- | --- | --- |
| 1 | Title | "GitHub Tutorial Project" | "GitHub Web Starter: Three Guides for Your First Repository" | Short, active | A reader should learn the outcome from the title, not the topic. |
| 2 | Section 1 | "The audience is students who want to learn GitHub." | A reader profile with four named limits (no Git vocabulary, clicks by label, two tabs one screen, first-try success) | One term for one thing | A named reader limits the writing. "Students who want to learn GitHub" would justify any guide about anything. |
| 3 | Section 2 | A paragraph describing the three tasks | A table with task, file, and status | Numbered steps, parallel form | The table answers "what do I get" in two seconds and shows which task is finished. |
| 4 | Section 2 | No exclusions | An explicit out-of-scope line (Git commands, pull requests, Pages, organisations, billing) | Short, active | A proposal is judged on whether the scope is manageable. Naming what is excluded proves it. |
| 5 | Guide 1, Step 2 | "click Add file" | "click the **Add file** dropdown, then choose **Create new file**" | Bold labels exactly | "Add file" alone does not say it is a menu, so the reader hunts for a button and misses the menu. |
| 6 | Guides 1–2 | "just click", "simply type", "very easy" | Deleted | No filler | These words blame the reader when a step fails, and they carry no instruction. |
| 7 | Guides 1–2 | "repo", "project", "folder" used for the same object | "repository", "file", "folder" used once each | One term for one thing | Three words for one object make the reader check whether they mean the same thing. |
| 8 | Both guides | Steps ended at "click the button" | Every guide ends with a Result Check of visible items | Verifiable result | A step is only done when the reader can see the result. "Click Commit changes" does not tell them what success looks like. |
| 9 | Section 4 | Word count decided after drafting | A word-count column in the plan table | 150–250 words | Writing to a number beats cutting afterwards. |
| 10 | Section 5 | Screenshots planned for every step | Screenshots dropped; labels bolded instead | Bold labels exactly | Screenshots age with every UI update and differ per account. A quoted label survives both. |

### 4. Uncertain facts

Everything here is a known gap, not a solved problem. The two guides are drafts until each row is closed.

| # | Uncertain fact | Where it appears | Status | How to close it |
| --- | --- | --- | --- | --- |
| 1 | Both guides were written from GitHub Docs. Neither has been clicked through end to end on a clean account. | Guides 1 and 2 | ⚠ Not yet verified by execution | Run both guides on a second account before calling them final. |
| 2 | The exact wording GitHub shows for a pending invitation on the **Collaborators** page. The docs page states that an email is sent, but does not quote the badge text, so the guide says "with a pending invitation" instead of quoting a label. | Guide 2, Result Check | ⚠ Unconfirmed | Send a test invitation, read the badge, then replace the paraphrase with the quoted label. |
| 3 | The tab that returns from **Preview** to editing. The docs quote **Preview** but not its partner tab, so the guide commits straight from preview. | Guide 1, Steps 5–6 | 🟡 Partially confirmed | Click through, note the label, and add the return step only if a reader needs it. |
| 4 | "**Commit changes** is greyed out when the file name field is empty." | Guide 1, "If a step fails" | 🟡 Observed behaviour, not documented | Reproduce it on a test repository. If it does not reproduce, delete the line. |
| 5 | "Free accounts can invite unlimited collaborators to a personal repository." True for repositories owned by a personal account; organisation repositories follow different limits. | Guide 2, Prerequisites | 🟡 Sourced, narrow | Keep the phrase "to a personal repository", and re-check after any plan change. |
| 6 | Word count depends on the counting method. `DOCUMENTATION_EDIT.docx` records 214 words for the Week 2 guide; `wc -w` returns 219, because it counts list markers and heading hashes as tokens. | Archive copy, plan table | ⚠ Method mismatch | State the counting method in each plan row, and count one way only. |
| 7 | The graded task uses a *private* repository, but this repository is public. The archived guide teaches the private-repository task; it does not claim this repository is private. | Archive guide | 🟡 Needs a reader check | Confirm the teacher reads the archive as a teaching copy, not as a description of this repository. |

### 5. What this pass did not change

The product, the three tasks, the task order, and every label quoted from GitHub Docs. Those were the fixed constraints, and an edit that broke one of them would not be a revision.

---

## Part 5 — Archive: frozen Week 2 tutorial

Appendix A reproduces the Week 2 practice tutorial word for word. Only the heading levels are one step deeper, so that the appendix sits under Part 5; no sentence changed. The untouched original is `README WEEK2.md`, which stays in the repository, and its SHA-256 is `0472d927b406c2fa31b9ebee86da182ee56e752d62a4d830664b88975334f86c`. Treat the appendix as frozen: an edited appendix is no longer a copy.

### Appendix A — How to Create a Private Repository with a README

Create a private GitHub repository with a default README in about two minutes.

#### Prerequisites

- A registered GitHub account at github.com
- Signed in to GitHub in a modern browser (Chrome, Edge, Firefox, or Safari)

#### Steps

1. **Open the new repository page.** In the upper-right corner of any GitHub page, click the **+** icon, then select **New repository** from the dropdown.
2. **Name your repository.** In the **Repository name** field, enter a repository name (for example, `my-private-project`). (Optional) Enter a description.
3. **Set the visibility to Private.** Under **Visibility**, select the **Private** radio button. Only you and people you invite can see the repository.
4. **Initialize with a README.** Check the **Add a README file** box to create a default README.md.
5. **Create the repository.** Click the green **Create repository** button.

#### Result Check

After the page reloads, confirm all four items on the repository main page:

- The repository name appears in the upper-left and matches the name you entered.
- A gray **Private** label appears next to the repository name.
- A file named README.md appears in the file list.
- The README content renders directly below the file list.

If all four items are visible, your private repository with a README was created successfully.

---

## AI disclosure

An AI assistant helped draft the structure, the phrasing, and the revision tables. I checked every quoted label against GitHub Docs myself, chose the scope and the reader profile, and made the final wording decisions. The items listed under "Uncertain facts" in Part 4 are open on purpose: they are the checks I have not finished, and I would rather record them than claim them.
