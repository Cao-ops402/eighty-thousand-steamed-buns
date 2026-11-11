# GitHub Web Starter: Three Guides for Your First Repository

A three-page documentation set that takes a first-year student from a new GitHub account to a shared, editable repository, using only the browser.

**Course:** Session 4 individual project proposal · **Author:** Cao-ops402 · **Repository:** [eighty-thousand-steamed-buns](https://github.com/Cao-ops402/eighty-thousand-steamed-buns)

---

## 1. Product, platform, and reader

| Item | Decision |
| --- | --- |
| **Product** | A documentation set of three task guides for the GitHub web interface. Each guide is one Markdown page of 150–250 words, ending with a Result Check. |
| **Platform** | GitHub in a desktop browser: Chrome, Edge, Firefox, or Safari. No command line, no GitHub Desktop, no mobile app. |
| **Target reader** | A first-year student with a new free GitHub account, no Git experience, and English as a second language. |

### Reader profile

The reader profile is written as constraints on the writing, not as a description of a market.

- **No Git vocabulary.** The reader knows "file" and "folder", not "commit", "branch", or "clone". Each term is defined at first use or avoided.
- **Clicks by label, not by memory.** The reader looks for the exact words on screen, so every on-screen label is bolded exactly as GitHub prints it.
- **Two tabs, one screen.** The guide sits in one tab, github.com in another. Each step must stand alone, because the reader cannot read step 4 while clicking step 1.
- **Success means first-try completion.** If the reader has to ask a classmate what to click next, the guide failed.

## 2. Task scope

Three related tasks on one ladder: **create → add → share**. Each task produces the input for the next, so the set is one project rather than three unrelated pages.

| # | Task | Guide | Status |
| --- | --- | --- | --- |
| 1 | Create a private repository with a README | [`archive/practice-tutorial/WEEK2 - Private Repository Tutorial.md`](<archive/practice-tutorial/WEEK2 - Private Repository Tutorial.md>) | Done in Weeks 1–2, frozen copy |
| 2 | Add a file to that repository in the browser | [`docs/GUIDE WEEK3 - Add a File in the Browser.md`](<docs/GUIDE WEEK3 - Add a File in the Browser.md>) | Draft, labels sourced |
| 3 | Invite a classmate as a collaborator | [`docs/GUIDE WEEK3 - Invite a Collaborator.md`](<docs/GUIDE WEEK3 - Invite a Collaborator.md>) | Draft, labels sourced |

**In scope:** one repository, one file, one collaborator, all through the web interface.

**Out of scope:** Git commands, pull requests, GitHub Pages, organisations, billing, and account recovery. Each is a separate task for a different reader, and each would double the length of the set.

## 3. README proposal

`README.md` at the repository root is the front door; this file is the proposal behind it. Both follow one rule: answer the reader's three questions in ten seconds.

1. **What is this?** A documentation set, not a program. The first line states the outcome, not the topic.
2. **Who is it for?** A named reader with named limits, so the writing has something to fail against.
3. **Where do I start?** The task table gives the order. A reader who only needs task 2 opens guide 2 and never reads guide 1.

The README leaves out installation steps, badges, licence text, and screenshots of the author's own account. None of them helps a first-year student click the next label.

## 4. Document plan

| File | Purpose | Words | Verification |
| --- | --- | --- | --- |
| `README WEEK3.md` | Proposal and index | 1,100–1,300 | Renders on GitHub; every link opens |
| `docs/GUIDE WEEK3 - Add a File in the Browser.md` | Task 2 guide | 150–250 | Click through on a clean account; 3 result items observed |
| `docs/GUIDE WEEK3 - Invite a Collaborator.md` | Task 3 guide | 150–250 | A classmate receives the invitation and opens the repository |
| `archive/practice-tutorial/WEEK2 - Private Repository Tutorial.md` | Frozen Week 2 guide | 219 | SHA-256 matches `archive/README.md`; file never edited |
| `docs/REVIEW WEEK3 - Constrained Edit.md` | Revision record | 1,100–1,300 | Every open fact listed with a way to close it |

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

## 5. Tool rationale

**Markdown in VS Code, with preview open.** Markdown is the format GitHub renders, so the file a reader opens is the page I write. A Word file would add a conversion step and break copy-paste of labels. Side-by-side preview catches heading-level mistakes before they reach a commit, and the Problems panel flags broken relative links between guides.

**Git and the GitHub web editor, one commit per guide.** A diff shows exactly which label changed between drafts, which is the only reliable way to keep a quoted label quoted. Uploading a finished .docx would replace the history with a single opaque file.

**`wc -w` for word count.** Counting is mechanical, so it should be done by a tool that always returns the same number. The catch: `wc -w` counts list markers and heading hashes as tokens, so the plan states the counting method once and uses it everywhere.

**GitHub Docs as the label source.** Every bolded label in guides 2 and 3 was read from a GitHub Docs page and recorded in `docs/REVIEW WEEK3 - Constrained Edit.md`, so any label can be traced back to its source sentence.

**Why not Word, Notion, or a wiki.** Each one renders its own page layout, and the reader would then learn that layout as well as GitHub's. The whole point of this set is that the reader learns one interface.

## 6. Repository

<https://github.com/Cao-ops402/eighty-thousand-steamed-buns>

The repository holds the documentation set, the archived practice tutorial, and the revision record. It is the only deliverable; no ZIP is needed because the whole set is versioned here.

## 7. AI disclosure

An AI assistant helped draft the structure, the phrasing, and the revision tables. I checked every quoted label against GitHub Docs myself, chose the scope and the reader profile, and made the final wording decisions. The items listed under "Uncertain facts" in `docs/REVIEW WEEK3 - Constrained Edit.md` are open on purpose: they are the checks I have not finished, and I would rather record them than claim them.
